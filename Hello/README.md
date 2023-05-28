# steps to fetch google calender events

>steps to create credentials and oauth 
Create the Oath Credentials & Oath Consent screen

In OAuth Consent Sceeen
 - Add the name & email id & user type & scope

Create the Credentials

- Click on create credentials
- Choose OAuth Client ID
- Choose Application Type as Web
- Give Name * Authorised Javascript origin as http://127.0.0.1:8000
- Add Authorised redirect uri http://127.0.0.1:8000/rest/v1/calendar/redirect/
- Save it and download the credential
- Rename the json as client_secret.json and add in same root as manage.py

> create a folder name django

> To create a virtual enviroment using the command
```
python -m venv env
.\env\Scripts\activate
```
> install the python packages using pip

>go inside the folder django
create a folder hello 

```
cd..
pip install google-auth google-auth-oauthlib
pip install django
```

```
django-admin startproject Hello
python manage.py startapp GoogeleCalendar
```
>run live server using the command
```
python manage.py runserver
```
Note:

change the secret key value in setting.py to secret value of your credentials

Change the client_secret.json file with your own json file downloaded




