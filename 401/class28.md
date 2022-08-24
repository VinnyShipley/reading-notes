# Django Forms

## What are django forms?

Django forms are a group of one or more fields/widgets on a webpage that all the user to submit information to the server.

## Creating a Form

### High Level

Devs need to first write the HTML for the form, validate and properly sanitize the entered data on the server, repost the form with the appropriate error messages to inform the user of any invalid field, handle the data when it is submitted successfully, and then finally respond to the user in some way that the form submission was a success

### Steps

* Create a Form class. This class needs to be imported from django. Similar to a Model class, the Form class needs specific attributes denoting wha kind of data it is taking i. Each form needs a form field, this controls what kind of input the form will take. Some kinds of inputs are:
  BooleanField, CharField, ChoiceField, TypedChoiceField, DateField, DateTimeField, DecimalField, DurationField, EmailField, FileField, FilePathField, FloatField, ImageField, IntegerField, GenericIPAddressField, MultipleChoiceField, TypedMultipleChoiceField, NullBooleanField, RegexField, SlugField, TimeField, URLField, UUIDField, ComboField, MultiValueField, SplitDateTimeField, ModelMultipleChoiceField, ModelChoiceField.

* Validate your data. One way to go about cleaning your input data is to create a clean_forms_name() function. The purpose of this function would be to validate that the input being given falls within the specific bounds of what you are trying to get from the user.

* Configure your URLs. Within the app that is using the form, you need to include the new form class in the path list to be redirected when they visit it.

* Configure your views. The view needs to be able to tell if it is being called for the first time, whether it is rendering an error message, or whether it is presenting the information it should when the information is valid.

* Configure the template for the form. Extend the ancestor class to a new html file, and input the data as you would normally in a django template.
