# Ex02 Django ORM Web Application
## Date: 
12.04.205
## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
=========

from django.db import models
from django.contrib import admin
class Movie(models.Model):
mid=models.IntegerField()
    mname=models.CharField(max_length=100)
    collection=models.IntegerField()
    year=models.IntegerField()
    rating=models.FloatField()

class MovieAdmin(admin.ModelAdmin):
    list_display=('mid','mname','collection','year','rating')


admin.py
=========

from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)
```


## OUTPUT

![Screenshot (145)](https://github.com/user-attachments/assets/f630b34e-3f94-4896-9647-8844f63b4ed2)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
