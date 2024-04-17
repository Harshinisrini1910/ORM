# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here
![image](https://github.com/selvasachein/ORM/assets/161415847/6c8fbfef-9849-47ee-846a-8f5e7bc3f592)

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
Models.py
```
from django.db import models
 from django.contrib import admin
 class Book_DB(models.Model):
  Booknum=models.IntegerField(primary_key="Booknum");
  title=models.CharField(max_length=15);
  Author=models.CharField(max_length=20);
  Date=models.DateField();
  lang=models.CharField(max_length=10);
  price=models.IntegerField();
 class Book_DBAdmin(admin.ModelAdmin):
Include the screenshot of your admin page.
 Thus the program for creating a database using ORM hass been executed successfully
  list_display=("Booknum","title","Author","Date","lang","price");
```
admin.py
```
from django.contrib import admin
 from .models import Book_DB,Book_DBAdmin
 admin.site.register(Book_DB,Book_DBAdmin)
```
## OUTPUT

Include the screenshot of your admin page.
![Screenshot 2024-04-17 at 9 05 29 AM](https://github.com/selvasachein/ORM/assets/161415847/5ac0153b-e70d-4d34-8aa4-674a4e6fad19)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
