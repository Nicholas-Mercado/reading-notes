# API Deployment

## Django Settings Best Practices

### Setting Configuration: Different Approaches

**settings_local**.py

Extend all environment specific settings in settings_local. set settings_local to be ignored by vcs

```py
ALLOWED_HOSTS = ['localhost']
DEBUG = True
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'local_db',
        'HOST': '127.0.0.1',
        'PORT': '5432',
    }
}
```

Pros

- secrets not in vcs

Cons

- its not in vcs so, potential to loose settings
- can have some non-obvious logic
- must have settings_local_example

**Separate settings file for each environment**

```py
python manage.py runserver --settings=settings.local
```

An extension of the settings_local.py. File structure like below

```py
settings/
   ├── __init__.py
   ├── base.py
   ├── ci.py
   ├── local.py
   ├── staging.py
   ├── production.py
   └── qa.py
```

Pros

- Everything stored in vcs.
- Easy to share

Cons

- Does nto handle secret passwords and tokens.
- Hard to trace and maintain

**Environment variables**

```py
import os


SECRET_KEY = os.environ['SECRET_KEY']
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': os.environ['DATABASE_NAME'],
        'HOST': os.environ['DATABASE_HOST'],
        'PORT': int(os.environ['DATABASE_PORT']),
    }
}
```

```python
import os

from django.core.exceptions import ImproperlyConfigured


def get_env_value(env_variable):
    try:
      	return os.environ[env_variable]
    except KeyError:
        error_msg = 'Set the {} environment variable'.format(var_name)
        raise ImproperlyConfigured(error_msg)


SECRET_KEY = get_env_value('SECRET_KEY')
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': get_env_value('DATABASE_NAME'),
        'HOST': get_env_value('DATABASE_HOST'),
        'PORT': int(get_env_value('DATABASE_PORT')),
    }
}
```

Pros

- Configuration is separate from your code
- Same code for all environments
- Cleaner code.

Cons

- Still must handle sharing default config
