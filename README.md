# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://github.com/Manoj0079940/ORM/assets/149366208/2b51c0d1-efb5-4839-b55d-4e73f7d76ecd)


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
admin.py
from django.contrib import admin
from .models import student,studentAdmin
admin.site.register(student,studentAdmin)

models.py
from django.db import models
from django.contrib import admin
class student (models.Model):
    name=models.CharField(max_length=20,help_text="student")
    rollno=models.IntegerField()
    refno=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class studentAdmin(admin.ModelAdmin):
    list_display=('name','rollno','refno','age','email')
```
## OUTPUT

![Screenshot 2024-04-03 203128](https://github.com/Manoj0079940/ORM/assets/149366208/2049d9d8-90dc-4b77-a3d2-39ba3627ff46)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
