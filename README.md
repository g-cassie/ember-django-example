This repo is an example of how to use the Django and Ember.js together,
taking advantage of the Django plugins, Django Rest Framework and
Ember-DRF.

I will try to add some informal documentation in this Readme. Hopefully
others will contribute.

## Creating a new app from scratch

The following terminal commands will get you a basic project structure
similar to the one used here.  It is assumed that you have pip and
virtualenv and ember-cli installed.  It is easy to google instructions
for installing each on your particular operating system. It is also
assumed that you have created a new repo for your project on github.

```
git clone <new repo url>

# create a virtual env for this project
# you may want to alternatively put your virtualenv in the project
# directory in which case you should make sure to .gitignore it.
virtualenv ~/virtualenvs/cars
source ~/virtualenvs/cars/bin/activate

# install the python dependencies
pip install Django
pip install djangorestframework
pip install emberdrf

# save these dependencies for easy installation later
pip freeze > requirements.txt

# start the django project and move it to the `django` folder
django-admin.py startproject cars
mv cars django

# start the ember project and move it to the `ember` folder
ember new cars
mv cars ember
```
