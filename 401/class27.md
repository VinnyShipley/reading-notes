# Django Models

## Using Models

Models allow a website to format information about an object a certain way, and then link those objects together in varying kinds of relationships

### Model Definition

To declare a model you create the model as a subclass of django.db.models.Models. The information contained within that subclass can then contain fields, methods, and metadata.

* Fields: Fields represent a column of data that we want to store in one of our database tables. Here are some of the kinds of inputs that a field can receive (list from [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)):

  * CharField is used to define short-to-mid sized fixed-length strings. You must specify the max_length of the data to be stored.

  * TextField is used for large arbitrary-length strings. You may specify a max_length for the field, but this is used only when the field is displayed in forms (it is not enforced at the database level).

  * IntegerField is a field for storing integer (whole number) values, and for validating entered values as integers in forms.

  * DateField and DateTimeField are used for storing/representing dates and date/time information (as Python datetime.date and datetime.datetime objects, respectively). These fields can additionally declare the (mutually exclusive) parameters auto_now=True (to set the field to the current date every time the model is saved), auto_now_add (to only set the date when the model is first created) , and default (to set a default date that can be overridden by the user).

  * EmailField is used to store and validate email addresses.

  * FileField and ImageField are used to upload files and images respectively (the ImageField adds additional validation that the uploaded file is an image). These have parameters to define how and where the uploaded files are stored.

  * AutoField is a special type of IntegerField that automatically increments. A primary key of this type is automatically added to your model if you don't explicitly specify one.

  * ForeignKey is used to specify a one-to-many relationship to another database model (e.g. a car has one manufacturer, but a manufacturer can make many cars). The "one" side of the relationship is the model that contains the "key" (models containing a "foreign key" referring to that "key", are on the "many" side of such a relationship).

  * ManyToManyField is used to specify a many-to-many relationship (e.g. a book can have several genres, and each genre can contain several books). In our library app we will use these very similarly to ForeignKeys, but they can be used in more complicated ways to describe the relationships between groups. These have the parameter on_delete to define what happens when the associated record is deleted (e.g. a value of models.SET_NULL would set the value to NULL).

* Metadata: To declare class level metadata, declare the subclass Meta within the class you would like to add metadata to. One of the most useful metadata applications is to control the order in which records will be returned hen you query the model type.

* Methods: Every model that you create should at the bare minimum have a string method that returns the field_name in a human readable form. Another common method is the get_absolute_string method which returns the url of that specific model instance.

### Model Management

Once the model class is defined you can use the CRUD process on them.

* To define an instance of a model, use the save() method.

* To search for records of the particular model, use the objects attribute. Use the all() method to search all of the objects of that kind.

* To filter out a specific kind of object type, use the filter() method with a particular parameter to only get the object that contains that parameter back from the query.

## Django Admin Site

The Django admin application allows you to build a site area that wil allow you to CRUD records. This allows for more effective testing in terms of if you are getting the right kind of data from the user in the site.

### Registering Models

Within the admin.py folder in the catalog application, import the models that you would like to register into the application by using admin.site.register(ModelName)

### Creating a Custom User

To log into the admin site, you need to create a user account with the staff status enabled. This will allow the user to view and create records, as well as manage the objects. To create a superuser that can do all of these things, in the command line run the prompt

      python3 manage.py createsuperuser

Then enter in a username, email, and strong password. Now restart the development server with the following command to test the login

      python3 manage.py runserver

### Logging in and Using the Site

Once logging into the admin url, the logged in superuser will then be able to create a new instance of the model you are trying to test.
