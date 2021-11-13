# Intro To Django


# What is Django ?

- Django is a high-level Python web framework that enables rapid development of secure and maintainable websites. Built by experienced developers, Django takes care of much of the hassle of web development, so you can focus on writing your app without needing to reinvent the wheel. It is free and open source, has a thriving and active community, great documentation, and many options for free and paid-for support.


# Why use Django ?

- Because Django helps developers by speeding up the development process. It includes its own Object Relation Mapping (ORM) layer for handling database access, sessions, routing, and multi-language support. It also takes care of security while handling requests. It includes an admin panel (called django-admin) for managing models data by default.

# Is Django Open Source & Who Maintains it ?

- Django’s code is open source and available to all. Django’s organization is managed by a non-profit, the DSF, with a miniscule budget. And Django code is lead by a core team of volunteers, two paid Django Fellows, and a larger group of contributors.

# Examples Of Using Django:

* Designing URLs for applications:

```python
from django.urls import path

from . import views

urlpatterns = [
    path('bands/', views.band_listing, name='band-list'),
    path('bands/<int:band_id>/', views.band_detail, name='band-detail'),
    path('bands/search/', views.band_search, name='band-search'),
]
```

```python
from django.shortcuts import render

def band_listing(request):
    """A view of all bands."""
    bands = models.Band.objects.all()
    return render(request, 'bands/band_listing.html', {'bands': bands})
      
```

* Forms with Django:

```python
from django import forms

class BandContactForm(forms.Form):
    subject = forms.CharField(max_length=100)
    message = forms.CharField()
    sender = forms.EmailField()
    cc_myself = forms.BooleanField(required=False)
```















[Go Back](https://musaabshalaldeh.github.io/reading-notes/)