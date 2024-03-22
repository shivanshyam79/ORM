# Ex02 Django ORM Web Application
## Date: 22/03/24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![WhatsApp Image 2024-03-19 at 10 57 49_e4af2a44](https://github.com/shivanshyam79/ORM/assets/151513860/e324eec5-c3f4-4443-ae81-22bf665945ee)


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
model.py

from django.db import models
from django.contrib import admin
class Railway_db(models.Model):
    trainno=models.IntegerField(primary_key=True);
    trainname=models.CharField(max_length=20);
    departure=models.CharField(max_length=50);
    arrival=models.CharField(max_length=50);
    distance=models.IntegerField();
class Railway_dbAdmin(admin.ModelAdmin):
    list_display=("trainno","trainname","departure","arrival","distance");

admin.py

from django.contrib import admin
from .models import Railway_db,Railway_dbAdmin
admin.site.register(Railway_db,Railway_dbAdmin)
```
## OUTPUT

![WhatsApp Image 2024-03-22 at 08 37 19_678d1b9c](https://github.com/shivanshyam79/ORM/assets/151513860/3bf80ab8-0094-4565-ade9-2b65f9268ac4)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
