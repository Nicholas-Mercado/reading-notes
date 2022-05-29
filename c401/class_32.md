# Permissions & Postgresql

## Django REST Framework

### DRF Permissions

Permission checks are run at the start of the view. No code will be run before this

Permission checks use the authentication information in the `request.user` and `request.auth` properties

#### How permissions are determined

Permissions in REST framework are defined as a list of permission classes

If permission is nto granted for any reason, an `exceptions.PermissionDenied` or `exceptions.NotAuthenticated` will be raised. No code will be run after

#### Object level permissions

REST framework support object-level permissioning

`.get_object()` - generic views is used to run Object level permissions

If writing your own views use `.check_object_permissions(request, obj)` method on the view

#### Setting the permission policy

default permission policy may be set globally, using the `DEFAULT_PERMISSION_CLASSES`

```py

REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}
```

using the APIView set the authentication policy on a per-view

```py
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

#### API Reference

AllowAny - Allows unrestricted access

IsAuthenticated - Will deny permission to any unauthenticated user

IsAdminUser - Will deny permission to any user, unless `user.is_staff` is `True`

IsAuthenticatedOrReadOnly - Will allow authenticated users access and unauthenticated users read only access

[Permissions](https://www.django-rest-framework.org/api-guide/permissions/)
