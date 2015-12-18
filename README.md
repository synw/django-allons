Django Mogo
==============

Starter kit for Django 1.8 projects.
This is a bunch of stuff put thogether to make a good starting base for new projects.

Features
--------------

This quick start kit installs the following Django modules:

- [django-allauth](https://github.com/pennersr/django-allauth) for authentication
- [django-alapage](https://github.com/synw/django-alapage) for pages management
- [django-jssor](https://github.com/synw/django-jssor) for slideshows management
- [django-zongo](https://github.com/synw/django-zongo) for responsive presentations
- [django-admin-bootstraped](https://github.com/django-admin-bootstrapped/django-admin-bootstrapped) for the admin interface

Base valid Xhtml 1.0 Strict templates using Bootstrap.
Some usefull generic css classes


Install
--------------

	pip install pillow django==1.8.7 django-debug-toolbar django-nose django-admin-bootstrapped django-bootstrap-form django-bootstrap3 django-mptt easy_thumbnails django-allauth django-ckeditor django-crispy-forms django-reversion

	cd path_to_your_project
	git clone https://github.com/synw/django-jssor.git && mv django-jssor/jssor . && mkdir media/jssor && mkdir media/jssor/thumbnails
	git clone https://github.com/synw/django-zongo.git && mv django-zongo/zongo . && mkdir media/zongo
	git clone https://github.com/synw/django-alapage.git && mv django-alapage/alapage .
	rm -rf django-jssor django-zongo django-alapage

Configure
--------------

Check the `sample_settings.py` file in the repository and tune your settings.py

Get the file `urls.py`

	python manage.py collectstatic

Get jquery and fontawesome icons:

	mkdir static && cd static && mkdir js && mkdir icons
	cd js && wget http://code.jquery.com/jquery-2.1.4.min.js
	cd ../icons && wget https://fortawesome.github.io/Font-Awesome/assets/font-awesome-4.5.0.zip
	unzip font-awesome-4.5.0.zip && mv font-awesome-4.5.0 font-awesome

Get the css from the `static/css` folder in the repository

Get the templates from the `templates` folder in the repository

	python manage.py migrate
	python manage.py createsuperuser
	python manage.py runserver

And go to `/admin` and start creating pages


Todo
--------------

- [ ] Package the whole thing in pip
- [x] Provide a base templates set
- [x] Provide default css generic classes

