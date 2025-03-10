# Ex02 Django ORM Web Application
## Date: 12.03.2024

## AIM
To develop a Django application to store and retrieve data from a Railway database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![WhatsApp Image 2024-03-19 at 10 43 37_74c3a80c](https://github.com/MabbuAdarsh/ORM/assets/149365583/de35d5a2-e487-4e6d-89f4-273c2305aa5a)

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

from .models import Train, TrainAdmin

admin.site.register(Train, TrainAdmin)

models.py

from django.db import models
from django.contrib import admin
class Train(models.Model):
    Train_code=models.CharField(max_length=20,primary_key=True)
    Train_name=models.CharField(max_length=100)
    start_time=models.DateTimeField()
    End_time=models.DateTimeField()
    start_station_code=models.CharField(max_length=20)
    End_station_code=models.CharField(max_length=20)
 
class TrainAdmin(admin.ModelAdmin):
    list_display=('Train_code','Train_name','start_time','End_time','start_station_code','End_station_code')

```
## OUTPUT

![WhatsApp Image 2024-03-19 at 11 08 38_6901a291](https://github.com/MabbuAdarsh/ORM/assets/149365583/f77cb96c-325b-4aee-8b02-592222bce2c9)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
