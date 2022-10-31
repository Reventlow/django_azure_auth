# django_azure_auth


Site setting are set to be uploaded to heroku. If you want to use this on your own server, you will need to change the settings.py file to point to your own server.

I have also included a requirements.txt file for heroku. If you are using your own server, you will need to install the requirements.txt file.

I have used the documentation from https://django-microsoft-auth.readthedocs.io/en/latest/usage.html to make the azure authentication work.

## Installation

### Heroku installation
Create a new app on heroku and add the following config vars
```
SECRET_KEY
MICROSOFT_AUTH_CLIENT_ID 
MICROSOFT_AUTH_CLIENT_SECRET  
MICROSOFT_AUTH_TENANT_ID 
```

### local installation
Local installation requires a .env file
```shell
SECRET_KEY = 
MICROSOFT_AUTH_CLIENT_ID = 
MICROSOFT_AUTH_CLIENT_SECRET = 
MICROSOFT_AUTH_TENANT_ID = 
```

create a virtual environment and run the following commands
```shell
pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```


