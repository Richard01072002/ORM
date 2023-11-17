# Ex02 Django ORM Web Application
## Date: 14.09.2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```
from django.db import models
from django.contrib import admin
class employement(models.Model):
    employementnumber = models.IntegerField(max_length=10)
    employementname = models.CharField(max_length=100)
    age = models.IntegerField() 
    email = models.EmailField()
    place = models.CharField(max_length=100)
    designation = models.CharField(max_length=100)
    salary = models.CharField(max_length=100)
class EmployementAdmin(admin.ModelAdmin):
    list_display = ('employementnumber','employementname','age','email','place','designation','salary')
```
## code in admin.py
```
from django.contrib import admin
from .models import employement,EmployementAdmin
admin.site.register(employement,EmployementAdmin)

```

## OUTPUT

![image](https://github.com/Richard01072002/ORM/assets/141472248/7ed48bd3-4946-462c-a24c-065436931943)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
