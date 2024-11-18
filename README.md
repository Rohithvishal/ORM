# Ex02 Django ORM Web Application
## Date:18/11/24

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![WhatsApp Image 2024-11-18 at 09 09 17_5e44d41b](https://github.com/user-attachments/assets/d8a7ab3b-681f-4f07-bcd5-bdd721d93bba)




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
from .models import Bank_loan,Bank_loanAdmin
admin.site.register(Bank_loan,Bank_loanAdmin)
```
model.py
```
from django.db import models
from django.contrib import admin
class Bank_loan(models.Model):
    Customer_Name=models.CharField(max_length=100)
    Customer_Age=models.IntegerField()
    Loan_Amount=models.IntegerField()
    Loan_Type=models.CharField(max_length=100)
    Loan_Duration=models.DateField()

class Bank_loanAdmin(admin.ModelAdmin):
    list_display=('Customer_Name','Customer_Age','Loan_Amount','Loan_Type','Loan_Duration')
```



## OUTPUT
![Screenshot 2024-11-18 090557](https://github.com/user-attachments/assets/e01f01b1-04ad-410a-bcf8-013cacd52024)
![Screenshot 2024-11-18 090613](https://github.com/user-attachments/assets/3329f543-8ff4-45b9-bf43-73e5346faba0)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
