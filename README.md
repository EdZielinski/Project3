# Pinocchio's Pizza & Subs  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This project is a pizza, subs and miscellaneous food ordering website, using Django 2.0.7, Python (3.7), Bootstrap (version 4), Django's templating system and Cascading Style Sheets (CSS3).

**Django admin**

* username - joe
* password - joe_pizza

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The creation of the superuser account with the following command  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>$python manage.py createsuperuser  

# Functionality, Key components and Design

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Django’s web framework is the driving design behind this web site.  Django is a heavy weight web framework that offers many out-of-the box features.  A description of the process of setting up the web site’s framework, functionality, key components and design follows.

**Setting up the website project's framework**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;To start a new project, the following command to give a folder structure framework of python files   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>$django-admin startproject pinocchios  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Next run the following command to create a folder that will create the main app of the project  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>$python manage.py startapp orders  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The above commands gave us the pinocchios folder and the orders folder

**pinocchios python files**

* Setting.py  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-There is a setting DEBUG=True that should be turned to false when delivered to production  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-Add the app orders to the installed apps with the setting 'orders.apps.OrdersConfig'  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the orders.py there is a file named apps.py that allows for the inheritance of this class from the orders app  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-The allowed hosts setting is set to ALLOWED_HOSTS = ['*']. Later this is set to the Domain name  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-This is also where you would set up the language, time zone, WSGI and static file folder name

**orders python files**

* urls.py

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- The urls.py The path function associates the route with the function and route.  It also gives an alias name to the location of the website page.  This is beneficial should you need to move the page around.  This alias name can be used in the HTML layout files, or HTML pages and be used throughout the program.

* models.py

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- The models.py This file is where data definitions are defined and registered.  We define classes here and inherit the template Models.Mode to take advantage of Django's ORM so no SQL is written.  This allows for abstraction of SQLite, MySQL, Postgres, NoSQL, or any other version of SQL on the market.  Djangos ORM handles this for any language.  The classes are defined as follows:

* admin.py

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- The admin.py file registers our classes defined in the models.py file.  The registration is necessary for us to administer these classes from the Administrative screen.  Each class must be registered in order for the superuser to manipulate the classes.  Django's Object Relational Model (ORM) does all the work necessary to present it to an Administrative Interface for the superuser.  

* views.py

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- The views.py file is where we house the functions that the user sees through our HTML pages associated with each function.  The functions in the pinocchio project are as follow:

**Requirements met**  



**Sources**

* The Django authentication system documentation  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://docs.djangoproject.com/en/2.0/topics/auth/default/  
* Models  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://docs.djangoproject.com/en/2.0/topics/db/models/  
* datetime - Basic date and time types from Python  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://docs.python.org/3/library/datetime.html  
* Admin  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://docs.djangoproject.com/en/2.0/ref/contrib/admin/  
* Models  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://docs.djangoproject.com/en/2.0/topics/db/models/  
* Request and response objects  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://docs.djangoproject.com/en/2.0/ref/request-response/  
* Django shortcut functions  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://docs.djangoproject.com/en/2.0/topics/http/shortcuts/  


