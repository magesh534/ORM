# Ex02 Django ORM Web Application
## Date: 28.02.2024
## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

















## Entity Relationship Diagram

![image](https://github.com/magesh534/ORM/assets/135577936/2fee9a8d-e027-4036-a2fd-d654b5c8ab3d)




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

```admin.py 

from django.contrib import admin
from .models import book_DB,book_DBAdmin
admin.site.register(book_DB,book_DBAdmin)

models.py
from django.db import models
from django.contrib import admin
class book_DB(models.Model):
    bookno=models.IntegerField(primary_key=True);
    bookname=models.CharField(max_length=10);
    authorname=models.CharField(max_length=10);
    yearofpublishing=models.DateField();
    pages=models.IntegerField();
    price=models.IntegerField();

class book_DBAdmin(admin.ModelAdmin):
   list_display=("bookno","bookname","authorname","yearofpublishing","pages","price");
```
## OUTPUT

![image](https://github.com/magesh534/ORM/assets/135577936/bd8ced8a-81e4-4c1d-a702-08ee1323dcc0)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
