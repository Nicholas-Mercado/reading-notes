# Intro to Django

## Getting started with Django

Django - web framework based in the python language

## urls and views

How to design urls for a application

Create module called URLconf.py

- This acts like a table of contents

```py

from django.urls import path

from . import views

urlpatterns = [
    path('bands/', views.band_listing, name='band-list'),
    path('bands/<int:band_id>/', views.band_detail, name='band-detail'),
    path('bands/search/', views.band_search, name='band-search'),
# ]  sets path of the url ..calls function in views


from django.shortcuts import render

def band_listing(request):
    """A view of all bands."""
    bands = models.Band.objects.all()
    return render(request, 'bands/band_listing.html', {'bands': bands})
```

[Great intro to views and urls](https://www.youtube.com/watch?v=TblSa29DX6I)

## Templates

```django
<html>
  <head>
    <title>Band Listing</title>
  </head>
  <body>
    <h1>All Bands</h1>
    <ul>
    {% for band in bands %}
      <li>                                          #Variables are surrounded by {{ and }}
        <h2><a href="{{ band.get_absolute_url }}">{{ band.name }}</a></h2>
        # Tags provide arbitrary logic in the rendering process
        # Some tags require ending tags like here-----------!
        {% if band.can_rock %}<p>This band can rock!</p>{% endif %}
      </li>
    {% endfor %}
    </ul>
  </body>
</html>
```

[Template Tags tutorial](https://www.youtube.com/watch?v=RCE3VUpzGw0)


