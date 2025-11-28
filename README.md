# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

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
admin.py
```
from django.contrib import admin
from .models import Car,CarAdmin
admin.site.register(Car,CarAdmin)
```
model.py
```
from django.db import models
from django.contrib import admin
class Car(models.Model):
    reg_no=models.CharField(max_length=100) 
    brandname = models.CharField(max_length=200)  
    fueltype =models.CharField(max_length=100)
    price=models.IntegerField()
    year=models.IntegerField()
    color=models.CharField(max_length=50)
class CarAdmin(admin.ModelAdmin):
    list_display=('reg_no',"brandname","fueltype",'price',"year",'color')
    ```

## OUTPUT
 <img width="1920" height="1080" alt="Screenshot (46)" src="https://github.com/user-attachments/assets/4f91be6e-b278-4fd0-a58c-71e6a0125b29" />




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
