# Ex02 Django ORM Web Application
# Date:02.12.2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2024-12-02 112533](https://github.com/user-attachments/assets/10a5d78b-c365-4e53-bec7-2dafef4e3a75)


## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM:
# admin.py
```
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)
```
# models.py
```
from django.db import models
from django.contrib import admin
class Bankloan (models.Model):
    Loanid=models.IntegerField(primary_key=True);
    Name=models.CharField(max_length=100);
    Age=models.IntegerField(default=18);
    Gender=models.CharField(max_length=1, default='M');
    City=models.CharField(max_length=20, default='Chennai');
    Accountno=models.IntegerField();
    Salary=models.IntegerField();
    Loanamt=models.IntegerField();

class BankloanAdmin(admin.ModelAdmin):
    list_display=('Loanid','Name','Age','Gender','City','Accountno','Salary','Loanamt')
```


# OUTPUT

![Screenshot 2024-12-02 112501](https://github.com/user-attachments/assets/3d404029-1aa0-41fc-994b-9e9c0aab4107)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
