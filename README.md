# Ex02 Django ORM Web Application
## Date: 12-04-25

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM)

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
from .models import footballplayer,footballplayerAdmin
admin.site.register(footballplayer,footballplayerAdmin)

models.py

from django.db import models
from django.contrib import admin
class footballplayer (models.Model):
    name=models.CharField(max_length=15)
    weight=models.IntegerField()
    age=models.IntegerField()
    members=models.CharField(max_length=20)
    experiance=models.IntegerField()

class footballplayerAdmin(admin.ModelAdmin):
    list_display=('name','weight','age','members','experiance')
```


## OUTPUT

![Screenshot 2025-04-12 102603](https://github.com/user-attachments/assets/de27ccd8-45da-48b8-83a9-2b50b4cf8159)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
