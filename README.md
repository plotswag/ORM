# Ex02 Django ORM Web Application
## Date: 14/09/2023

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

## PROGRAM:
```
Admin.py

from django.contrib import admin
from .models import footballplayer,footballplayerAdmin
admin.site.register(footballplayer,footballplayerAdmin)

Models.py

from django.db import models
from django.contrib import admin
class footballplayer (models.Model):
    numofmatch=models.IntegerField()
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    height=models.IntegerField()

class footballplayerAdmin(admin.ModelAdmin):
    list_display=('numofmatch','name','salary','age','height')

```

## OUTPUT
![Screenshot 2023-11-17 120158](https://github.com/plotswag/ORM/assets/145822344/bed57bb3-7bbb-480d-8d47-e97f6e9b5dcf)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
