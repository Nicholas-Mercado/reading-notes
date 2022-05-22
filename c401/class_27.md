# Django Models

## Using Models

models - Python objects that Django web applications use to access and manage data through

- Django allows you to choose a database then do all the interactions with models

## Designing Models

When designing your models you should have separate models for every object

Django allows you to define relastionships in these ways

- one to one (OneToOneField)
- one to many (ForeignKey)
- many to many (ManyToManyField)

```py

import Django.db import Models

class Article(models.Model):
    title = models.CharField()
    body = models.TextField()
    date = DateTimeField(auto_now_add=True)
```

[Model field reference](https://docs.djangoproject.com/en/1.11/ref/models/fields/)

[Django Tutorial #6 - Django Models](https://www.youtube.com/watch?v=5zNR3E6WRLE)

## Django admin site

Django admin application - automatically builds a site area in your site that you can use to create, view, update, and delete records.

### Registering models

Import

```py
from django.contrib import admin
from .models import #model/names

admin.site.register(model/name)
```
