# Academlo-Library


REST-API based in a library, where the users can rent and to see all avaible books, this app is developed with Django-Rest-Framework.


## Table of Contents


- [Installation](#installation)
- [Usage](#usage)
- [Endpoints y Admin](#endpoints)
- [SwaggerUI y JWT](#swaggerui)

## Installation 
-Clone the repository 
-Create your virtual environment 
-Activate your virtual environment
-Execute the follow comand
pip install -r requirements.txt // install all the requirements
```
## Usage
 Create the DB and run the migrations

If you wanna run the api in local host you need to create a DB in postgress and to call to you BD as "library-api", 
then you need to make migrations "py manage.py migrate"


You can see you DB with pg-admin.

Remember to run the command py manage.py makemigrations


### Endpoints


You can see all the urls or endpoint with this URI " http://127.0.0.1:8000/api/schema/swagger-ui/"


For to start the api first you need to make and superuser with the follow command ```py manage.py createsuperuser ``` after that you need to open
the follow URL ```http://localhost:8000/admin ``` write your credentials and in the framework you can create, modify and delete dates.


### SwaggerUI
After to create the superuser, you can sign up with your credentials in the follow url for to generate your token "http://localhost:8000/api/token/ "
this this token you can make petitions as post, get or delete, you can make it with "postman".

also you can make autorization or to run the methods in Swagger Ui just open the follow url
```http://127.0.0.1:8000/api/schema/swagger-ui/ ``` and press in the button "authorize and sign up with the token that you generated before.

