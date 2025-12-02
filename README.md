# Ex01 Django ORM Web Application
## Date: 

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM
Models.py
from django.db import models
from django.contrib import admin

class Customer(models.Model):

    regid = models.CharField(max_length=20, help_text="regestried ID")
    name = models.CharField(max_length=100)
    price = models.IntegerField()
    year = models.IntegerField()

class CustomerAdmin(admin.ModelAdmin):

    list_display = ('regid', 'name', 'price', 'year')

admin.py
from django.contrib import admin
from.models import Customer,CustomerAdmin
admin.site.register(Customer,CustomerAdmin)




## OUTPUT
<img width="1246" height="604" alt="Screenshot 2025-12-02 230408" src="https://github.com/user-attachments/assets/ab8989f6-e7c1-4e29-8691-14c349013686" />



## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
