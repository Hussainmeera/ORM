# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/6da3ecbb-d3b3-46fe-af7b-e97d6d490560)




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

from django.db import models
from django.contrib import admin 
class BankLoan(models.Model):
  acc=models.IntegerField(primary_key="accno")
  ph=models.IntegerField()
  ifsc=models.CharField(max_length=100)
  loanno=models.IntegerField()
  adress=models.CharField(max_length=100)
  pan=models.IntegerField()
  adhar=models.IntegerField()

class BankLoanAdmin(admin.ModelAdmin):
 list_display=('acc','ph','ifsc','loanno','adress','pan','adhar',)

 admin.py

 from django.contrib import admin
from .models import BankLoan,BankLoanAdmin
admin.site.register(BankLoan,BankLoanAdmin)

```



## OUTPUT
![Screenshot (4)](https://github.com/user-attachments/assets/0367afa7-d4da-4b1f-a12e-572105a2f22a)
![Screenshot (5)](https://github.com/user-attachments/assets/a28e5140-3967-49fb-b9b2-c07f5510bb2e)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
