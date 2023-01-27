# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![er diagram](https://user-images.githubusercontent.com/118707347/215138423-0b5f9e9d-c601-44cb-a32a-e29a1c7133ba.png)

## DESIGN STEPS!

### STEP 1:

Create the django domain

### STEP 2:

Then from the the django.db import the models and then from the django.contribute import the admin
### STEP 3:

Superuser is created successfully.

## PROGRAM
```
models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('username','email address','first name','last name','Staff status')

admin.py
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```

## OUTPUT

![22009131 (2)](https://user-images.githubusercontent.com/118707347/215141282-d07e1f23-7d92-4126-90c1-34683d2d4589.png)

## RESULT
Program  Was executed successfully.

