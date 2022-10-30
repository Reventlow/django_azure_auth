release: python manage.py migrate
web: gunicorn django_azure_auth.wsgi --log-file -
clock: python clock.py