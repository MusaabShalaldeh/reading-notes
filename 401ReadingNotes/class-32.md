# Permissions in Django REST Framework



### What are Permissions?

- In general, permissions are access details given by users or network administrators that define access rights to files on a network.

### Why are Permissions used ?

- Permissions are used to grant or deny access for different classes of users to different parts of the API.

### When do Permission checks run ?

- Permission checks are always run at the very start of the view, before any other code is allowed to proceed.

### How permissions are determined?

- Permissions in REST framework are always defined as a list of permission classes.

### When the permissions checks fail either a "403 Forbidden" or a "401 Unauthorized" response will be returned, according to the following rules:

- The request was successfully authenticated, but permission was denied. — An HTTP 403 Forbidden response will be returned.
- The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers. — An HTTP 403 Forbidden response will be returned.
- The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers. — An HTTP 401 - Unauthorized response, with an appropriate WWW-Authenticate header will be returned.

### Setting the permission policy:

he default permission policy may be set globally, using the DEFAULT_PERMISSION_CLASSES setting. For example.

```python
REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}
```

If not specified, this setting defaults to allowing unrestricted access:

```python
'DEFAULT_PERMISSION_CLASSES': [
   'rest_framework.permissions.AllowAny',
]
```

You can also set the authentication policy on a per-view, or per-viewset basis, using the APIView class-based views.

```python
from rest_framework.permissions import IsAuthenticated
from rest_framework.response import Response
from rest_framework.views import APIView

class ExampleView(APIView):
    permission_classes = [IsAuthenticated]

    def get(self, request, format=None):
        content = {
            'status': 'request was permitted'
        }
        return Response(content)
```
Or, if you're using the @api_view decorator with function based views.

```python
from rest_framework.decorators import api_view, permission_classes
from rest_framework.permissions import IsAuthenticated
from rest_framework.response import Response

@api_view(['GET'])
@permission_classes([IsAuthenticated])
def example_view(request, format=None):
    content = {
        'status': 'request was permitted'
    }
    return Response(content)
```

Note: when you set new permission classes via the class attribute or decorators you're telling the view to ignore the default list set in the settings.py file.

Provided they inherit from rest_framework.permissions.BasePermission, permissions can be composed using standard Python bitwise operators. For example, IsAuthenticatedOrReadOnly could be written:

```python
from rest_framework.permissions import BasePermission, IsAuthenticated, SAFE_METHODS
from rest_framework.response import Response
from rest_framework.views import APIView

class ReadOnly(BasePermission):
    def has_permission(self, request, view):
        return request.method in SAFE_METHODS

class ExampleView(APIView):
    permission_classes = [IsAuthenticated|ReadOnly]

    def get(self, request, format=None):
        content = {
            'status': 'request was permitted'
        }
        return Response(content
```


### API References:

* AllowAny
```
The AllowAny permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.

This permission is not strictly required, since you can achieve the same result by using an empty list or tuple for the permissions setting, but you may find it useful to specify this class because it makes the intention explicit.
```
* IsAuthenticated
```
The IsAuthenticated permission class will deny permission to any unauthenticated user, and allow permission otherwise.

This permission is suitable if you want your API to only be accessible to registered users.
```
* IsAdminUser
```
The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.

This permission is suitable if you want your API to only be accessible to a subset of trusted administrators.
```
* IsAuthenticatedOrReadOnly
```
The IsAuthenticatedOrReadOnly will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.

This permission is suitable if you want to your API to allow read permissions to anonymous users, and only allow write permissions to authenticated users.
```
* DjangoModelPermissions
```
This permission class ties into Django's standard django.contrib.auth model permissions. This permission must only be applied to views that have a .queryset property or get_queryset() method. Authorization will only be granted if the user is authenticated and has the relevant model permissions assigned.

POST requests require the user to have the add permission on the model.
PUT and PATCH requests require the user to have the change permission on the model.
DELETE requests require the user to have the delete permission on the model.
The default behaviour can also be overridden to support custom model permissions. For example, you might want to include a view model permission for GET requests.

To use custom model permissions, override DjangoModelPermissions and set the .perms_map property. Refer to the source code for details.
```
* DjangoModelPermissionsOrAnonReadOnly
```
Similar to DjangoModelPermissions, but also allows unauthenticated users to have read-only access to the API.
```

* DjangoObjectPermissions
```
This permission class ties into Django's standard object permissions framework that allows per-object permissions on models. In order to use this permission class, you'll also need to add a permission backend that supports object-level permissions, such as django-guardian.

As with DjangoModelPermissions, this permission must only be applied to views that have a .queryset property or .get_queryset() method. Authorization will only be granted if the user is authenticated and has the relevant per-object permissions and relevant model permissions assigned.

POST requests require the user to have the add permission on the model instance.
PUT and PATCH requests require the user to have the change permission on the model instance.
DELETE requests require the user to have the delete permission on the model instance.
Note that DjangoObjectPermissions does not require the django-guardian package, and should support other object-level backends equally well.

As with DjangoModelPermissions you can use custom model permissions by overriding DjangoObjectPermissions and setting the .perms_map property. Refer to the source code for details.
```







[Go Back](https://musaabshalaldeh.github.io/reading-notes/)