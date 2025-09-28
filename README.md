# Ex02 Django ORM Web Application
# Date:28/09/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
from django.db import models
from django.contrib import admin
class car(models.Model):
    car_brand=models.CharField(max_length=20)
    car_model=models.CharField(max_length=20)
    mileage=models.IntegerField()
    engine_type=models.CharField(max_length=20)
    manfg_date=models.DateField()
class caradmin(admin.ModelAdmin):
    list_display=('car_brand','car_model','mileage','engine_type','manfg_date')

from django.contrib import admin
from .models import car,caradmin
admin.site.register(car,caradmin)
```
# OUTPUT
<img width="1059" height="498" alt="output" src="https://github.com/user-attachments/assets/0772f8c5-8747-494b-9a14-1825756325a2" />



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
