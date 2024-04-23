# Ex02 Django ORM Web Application
## Date: 16/04/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://github.com/Harshinisrini1910/ORM/assets/161415847/2a2b07ce-9e61-4cdb-bf97-e1ca7d306787)


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
```
models.py

from django.db import models
from django.contrib import admin
class Books(models.Model):
	bookno         = models.IntegerField(primary_key=True);
	bookname       = models.CharField(max_length=20);
	author         = models.CharField(max_length=20);
	pages          = models.IntegerField();
	published_date = models.DateField();
	bookprice      = models.IntegerField();
class BooksAdmin(admin.ModelAdmin):
	list_display=("bookno","bookname","author","pages","published_date","bookprice");

admin.py
	
from django.contrib import admin
from.models import Books,BooksAdmin
admin.site.register(Books,BooksAdmin)
```

## OUTPUT

![image](https://github.com/Harshinisrini1910/ORM/assets/161415847/7e54630d-8e4d-4fd4-b683-1021321031b8)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
