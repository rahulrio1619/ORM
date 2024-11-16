# Ex02 Django ORM Web Application
## Date: 16/11/2024
RAHUL RIO S

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![WhatsApp Image 2024-11-16 at 14 09 19_ec986d8e](https://github.com/user-attachments/assets/43083ad7-86d3-4abe-8067-9f9418b6520b)



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
class LoanDB(models.Model):
    Customer_ID=models.IntegerField(primary_key=True)
    Customer_name=models.CharField(max_length=100)
    Loan_no=models.IntegerField()
    Loan_amount=models.IntegerField()
    Mail_ID=models.EmailField()

class LoanDBAdmin(admin.ModelAdmin):
     list_display=('Customer_ID','Customer_name','Loan_no','Loan_amount','Mail_ID')

admins.py

from django.contrib import admin
from .models import LoanDB, LoanDBAdmin

admin.site.register(LoanDB, LoanDBAdmin)


```

## OUTPUT
![Screenshot (48)](https://github.com/user-attachments/assets/2cf9f76d-547d-4301-8c1f-0dfa0ac95b3c)
![Screenshot (47)](https://github.com/user-attachments/assets/85260c66-ff71-4d45-901f-8362020596f4)






## RESULT
Thus the program for creating a database using ORM hass been executed successfully
