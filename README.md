# Django Argon

**Modern template for Django interface** coded in **Django Framework** by **AppSeed** [App Generator](https://appseed.us/app-generator)

<br>

## Why Django Argon?
- UI Kit: **Argon Dashboard** (Free version) provided by **Creative-Tim**
- New fresh look
- Responsive mobile interface
- Minimal template overriding
- Easy integration

<br />

## Screenshots

![Django Argon - Template project provided by AppSeed.](https://s3.amazonaws.com/creativetim_bucket/products/336/original/opt_ad_django_thumbnail.jpg)

<br>

## Installation

```bash
$ pip install git+https://github.com/app-generator/django-argon.git
$ # or
$ easy_install git+https://github.com/app-generator/django-argon.git
```

* Add `argon` application to the INSTALLED_APPS setting of your Django project settings.py file:

```python
    INSTALLED_APPS = (
        ...
        'argon'
    )
```


* Make sure ``django.template.context_processors.request`` context processor is enabled in settings.py (Django 1.8+ way):

```python

    TEMPLATES = [
        {
            'BACKEND': 'django.template.backends.django.DjangoTemplates',
            'DIRS': [],
            'APP_DIRS': True,
            'OPTIONS': {
                'context_processors': [
                    ...
                    'django.template.context_processors.request',
                    ...
                ],
            },
        },
    ]
```

:warning: **Warning!!**
* Before Django 1.8 you should specify context processors different way. Also use ``django.core.context_processors.request`` instead of ``django.template.context_processors.request``.

```python
    from django.conf import global_settings

    TEMPLATE_CONTEXT_PROCESSORS = global_settings.TEMPLATE_CONTEXT_PROCESSORS + (
        'django.core.context_processors.request',
    )
```

* Collect static if you are in production environment:

```bash
$ python manage.py collectstatic
```

* Clear your browser cache

<br />

## More Details

### [Django Argon](https://github.com/app-generator/django-argon)

Start fast your next Django project by using functional django argon.

### [Django Argon](https://www.creative-tim.com/product/argon-dashboard-django?AFFILIATE=128200)

**[Django Argon](https://www.creative-tim.com/product/argon-dashboard-django?AFFILIATE=128200)** is a beautiful Bootstrap 4 Admin Dashboard with a huge number of components built to fit together and look amazing. If you are looking for a tool to manage and visualize data about your business, this dashboard is the thing for you. It combines colors that are easy on the eye, spacious cards, beautiful typography, and graphics.

<br />

---
**Django Argon** - Provided by **AppSeed** [App Generator](https://appseed.us/app-generator).
