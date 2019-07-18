===================
django-csrf-view
===================

Simple view for get csrf token in json response.

Install
-------------------

`pip3 install django-csrf-view`

How to use it?
---------------------

Use view in your urlpatterns:

.. code-block:: python

    from django.urls import path
    from django_csrf_view import CSRFView

    urlpatterns = [
        path('csrf/', CSRFView.as_view()),
    ]

And get your csrf:

`curl http://localhost:8000/api/v01/csrf/`
`{"token": "r2OoVhaNjECZjoBl8hwcgulE5ULgyaVv0hbWtX1SBZ8M263GQHJS8ZyNHwN0Y4ZI"}`
