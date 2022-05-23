# Django Custom User

## Django Custom User Model

Django has a built in user model for authentication.

see tutorial [here](https://learndjango.com/tutorials/django-login-and-logout-tutorial)

Django recommends always using a custom user model for new projects

link to setup [here](https://learndjango.com/tutorials/django-custom-user-model)

### AbstractUser vs AbstractBaseUser

There are two modern ways to create custom user models

AbstractBaseUser - requires so much more work

AbstractUser - is more of a default configuration

### Creating a custom user model

This requires four steps

- update django_project/settings.py
- create a new CustomUser model
- create new UserCreation and UserChangeForm
- update the admin

## Abstract User, User Profile and Signals in Django

All Django applications have a user model by default

includes:

- Email
- Username
- password
- Storage Quota
- Picture

How to add extra fields to model

```py
import django.contrib.auth.models AbstractUser
# Add extra fields to user model

class User(AbstractUser):
    quota = models.IntegerField()
```

```py
settings.AUTH_USER_MODEL
```

[Abstract User, User Profile and Signals in Django](https://www.youtube.com/watch?v=EudKs1HPUfE)



