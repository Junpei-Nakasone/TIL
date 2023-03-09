NOTE: If you deploy your DRF to production, you should use environment variable for django secret_key in `settings.py`.

```bash
python3 --version
```


```bash
pip3 list
```

```bash
pip3 install django
```

```bash
pip3 install djangorestframework
```

```bash
pip3 list
```

```bash
django-admin startproject server
```

```bash
cd server
server  manage.py
```

```bash
python manage.py startapp jsonplaceholder
```

```bash
ls -la
total 4
drwxr-xr-x 5 vscode vscode 160 Jan 28 21:25 .
drwxr-xr-x 8 vscode vscode 256 Jan 28 21:23 ..
drwxr-xr-x 9 vscode vscode 288 Jan 28 21:25 jsonplaceholder
drwxr-xr-x 7 vscode vscode 224 Jan 28 21:23 server
-rwxr-xr-x 1 vscode vscode 666 Jan 28 21:23 manage.py
```

server/settings.py
```python
INSTALLED_APPS = [
    "django.contrib.admin",
    "django.contrib.auth",
    "django.contrib.contenttypes",
    "django.contrib.sessions",
    "django.contrib.messages",
    "django.contrib.staticfiles",
    "jsonplaceholder", # add
    "rest_framework", # add
]
```

jsonplaceholder/models.py
```python
from django.db import models

# add User class
class User(models.Model):
    name = models.CharField(max_length=100)
    username = models.CharField(max_length=100)
    email = models.EmailField(max_length=100, unique=True)

```

```bash
python manage.py makemigrations
```

```bash
python manage.py migrate
```

```bash
python manage.py createsuperuser --email admin@example.com --username admin
```

```bash
touch server/jsonplaceholder/serializers.py
```

```bash
code server/jsonplaceholder/serializers.py
```

server/jsonplaceholder/serializers.py
```python
from rest_framework import serializers
from jsonplaceholder.models import User

class UserSerializer(serializers.ModelSerializer):
    class Meta:
        model = User
        fields = '__all__'


```

```bash
touch server/jsonplaceholder/api.py
```

```bash
code server/jsonplaceholder/api.py
```

```python
from jsonplaceholder.models import User
from rest_framework import viewsets, permissions
from .serializers import UserSerializer

class UserViewSet(viewsets.ModelViewSet):
    queryset = User.objects.all()
    permission_classes = [
        permissions.AllowAny
    ]
    serializer_class = UserSerializer
```

```bash
code server/urls.py
```

server/urls.py
```python
from django.contrib import admin
from django.urls import path, include

urlpatterns = [
    path("", include('jsonplaceholder.urls')),
]
```

```bash
touch server/jsonplaceholder/urls.py
```

```bash
code server/jsonplaceholder/urls.py
```

server/jsonplaceholder/urls.py
```python
from rest_framework import routers
from .api import UserViewSet

router = routers.DefaultRouter()
router.register('api/users', UserViewSet, 'users')

urlpatterns = router.urls
```

```bash
python manage.py runserver
```

VSCode REST Client
```json
GET http://localhost:8000/api/users/
[]
```

```json
###
POST http://localhost:8000/api/users/
Content-Type: application/json

{
    "name": "name",
    "username": "username",
    "email": "test@email.com"
}
```

```json
###
POST http://localhost:8000/api/users/
Content-Type: application/json

{
    "name": "name2",
    "username": "username2",
    "email": "test2@email.com"
}
```

```bash
GET http://localhost:8000/api/users/
[
  {
    "id": 1,
    "name": "name",
    "username": "username",
    "email": "test@email.com"
  },
  {
    "id": 2,
    "name": "name2",
    "username": "username2",
    "email": "test2@email.com"
  }
]
```

```bash
GET http://localhost:8000/api/users/1
  {
    "id": 1,
    "name": "name",
    "username": "username",
    "email": "test@email.com"
  }
```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```

```bash

```
