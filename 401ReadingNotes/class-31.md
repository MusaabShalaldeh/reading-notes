# Docker



### What is Docker ?

- Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels. 

### Why use Docker ?

- Because Docker enables developers to easily pack, ship, and run any application as a lightweight, portable, self-sufficient container, which can run virtually anywhere. As Bottomley told me, "Containers gives you instant application portability."

### Getting Started With Docker:

To install Docker we need to download the desktop app on our computer and create a free account. The initial download of Docker might take some time to download.

Once Docker is done installing we can confirm the correct version is running. It should be at least version 19.

```bash
$ docker --version
Docker version 19.03.5, build 633a0ea
```

Docker Compose is an additional tool that is automatically included with Mac and Windows downloads of Docker. However if you are on Linux, you will need to add it manually. You can do this by running the command sudo pip install docker-compose after your Docker installation is complete.

Now run the command below to confirm you have a working version of it, too. The version should be at least 1.24.x.

```bash
$ docker-compose --version
docker-compose version 1.24.1, build 4667896b
```

### What are the important fundamentals to understand when starting with Docker ?

- Images and containers are the two fundamental concepts to grasp when you start with Docker. An image is a snapshot in time of what a project contains. A container is a running instance of the image.


# Django REST Framework


### What is Django REST Framework ?

- Django REST framework is a powerful and flexible toolkit for building Web APIs. Some reasons you might want to use REST framework: The Web browsable API is a huge usability win for your developers. Authentication policies including packages for OAuth1a and OAuth2.

### Why use Django REST Framework ?

- Because it makes serialization so easy! In Django, you define your models for your database using Python. While you can write raw SQL, for the most part the Django ORM handles all the database migrations and queries.


### How to add Django REST Framework ?

- Django REST Framework is added just like any other third-party app. Make sure to quit the local server Control + c if it is still running. Then on the command line type the below.

```bash
(library) $ poetry add djangorestframework~=3.11.0
```

Then Add it to the INSTALLED_APPS config in our settings.py file. I like to make a distinction between third-party apps and local apps as follows since the number of apps grows quickly in most projects.

config/settings.py
```python
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',

    # 3rd party
    'rest_framework', # new

    # Local
    'books',
]
```

[Go Back](https://musaabshalaldeh.github.io/reading-notes/)