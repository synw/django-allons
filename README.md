# Django Mogo

Starter kit for Django projects. This is a bunch of stuff put thogether to make a ready to use Django environment.

Mogo installs a set of Python and Django modules as well as some static stuff ( bootstrap, jquery ) 
and base templates. It also autogenerates a settings file.

## Requirements

Virtualenv, pip, git and the necessary packages to install Pillow

## Features

This quick start kit installs the following Django modules:

#### Image processing

- [pillow](https://github.com/python-pillow/Pillow): standard image processing lib
- [easy-thumbnails](https://github.com/SmileyChris/easy-thumbnails): generate thumbnails using cache

#### Authentication

- [django-allauth](https://github.com/pennersr/django-allauth) for authentication with social networks

#### Text editors

- [django-ckeditor](https://github.com/django-ckeditor/django-ckeditor): wysywig text editor
- [django-codemirror2](https://github.com/sk1p/django-codemirror2): code editor

#### Content management

- [django-filer](https://github.com/divio/django-filer): files management
- [django-spages](https://github.com/synw/django-spages) for pages management
- [django-qcf](https://github.com/synw/django-qcf): contact form
- [django-userprofiles](https://github.com/synw/django-userprofiles): user profiles for django-allauth

#### Utilities

- [ipython](http://ipython.org/) : powerfull python shell integrated with Django
- [pytz](http://pytz.sourceforge.net/): timezones
- [django-compressor](https://github.com/django-compressor/django-compressor): to compress static assets
- [django-reversion](https://github.com/etianen/django-reversion) for version control
- [django-mptt](https://github.com/django-mptt/django-mptt): utility for working with trees
- [django-braces](https://github.com/brack3t/django-braces): usefull mixins
- [django-extensions](https://github.com/django-extensions/django-extensions) : usefull tools
- [django-mqueue](https://github.com/synw/django-mqueue): for logging app events 
- [django-system-monitor](https://github.com/hakanzy/django-system-monitor): for monitoring the system load
- [django-dirtyedit](https://github.com/synw/django-dirtyedit): uility for editing files in the admin interface

#### Bootstrap stuff

- [django-bootstrap-form](https://github.com/tzangms/django-bootstrap-form)
- [django-bootstrap3](https://github.com/dyve/django-bootstrap3)

#### Test / debug

- [django-debug-toolbar](https://github.com/django-debug-toolbar/django-debug-toolbar) for apps debug
- [pytest-django](https://github.com/pytest-dev/pytest-django): test suite
- [pytest-cov](https://github.com/pytest-dev/pytest-cov): coverage for pytest
- [coverage](https://bitbucket.org/ned/coveragepy): utility for test coverage reporting
- [django-autofixture](https://github.com/gregmuellegger/django-autofixture): for generating test data

#### Static files

Batteries are included:

- Jquery
- Base template set using Bootstrap

## Install

Note you will need virtualenv, git and a few libs installed on your system before to install, such as the ones required
for Pillow.

  ```bash
git install git+https://github.com/synw/django-mogo.git
# cd to a dir where you want your virtual env and the django project to be installed
# do not set a virtualenv: Mogo will do it for you
python djangomogo
  ```

Tweak the autogenerated `settings.py` to fit your needs.

### Install options

Django only:

   ```bash
python djangomogo -django
   ```
