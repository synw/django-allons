# Django Mogo

Starter kit for Django projects. Installs a ready to use Django environment with utility modules and
templates, autogenerating a settings file.

## What you get

- A ready to use Django environnement with a complete set of utilities
- Single page app Vue.js frontend with [Vite Vue](https://github.com/synw/django-vitevue)
- Websockets ready with [Django Instant](https://github.com/synw/django-instant), 
powered by [Centrifugo](https://github.com/centrifugal/centrifugo/)

## Requirements

Virtualenv, pip, git and the necessary packages to install Pillow

## Install

Note you will need virtualenv, git and a few libs installed on your system before to install, such as the ones required
for Pillow.

  ```bash
git install git+https://github.com/synw/django-mogo.git
# cd to a dir where you want your virtual env and the django project to be installed
# do not set a virtualenv: Mogo will do it for you
python3 djangomogo
  ```

Tweak the autogenerated `settings.py` to fit your needs.

### Install options

The base installer will setup Django with a bunch of modules. It will ask for installing pages management package, 
contact form (all integrated in a Vue.js frontend), and the realtime modules for websockets. 
The following install options are available

Django only:

   ```bash
python3 djangomogo -django
   ```

Do not install and configure Django, just install modules:

   ```bash
python3 djangomogo -modules
   ```
   
Install more modules:

   ```bash
python3 djangomogo -plus
   ```

Ask more questions about what modules to install

   ```bash
python3 djangomogo -prompt
   ```
   
Install the developement modules: pytest, coverage and the Grunt assets pipeline (npm is required)

   ```bash
python3 djangomogo -dev
   ```

## Applications list

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

- [django-vitevue](https://github.com/synw/django-vitevue) to manage the Vue.js frontend
- [django-vvpages](https://github.com/synw/django-vvpages) for pages management
- [django-vvcontact](https://github.com/synw/django-qcf): contact form
- [django-vvcatalog](https://github.com/synw/django-vvcatalog): products catalog (optional)

#### Websockets (optional)

- [Centrifugo](https://github.com/centrifugal/centrifugo/): the websockets server
- [django-instant](https://github.com/synw/django-instant): Centrifugo <-> Django layer
- [django-presence](https://github.com/synw/django-presence) to manage the Vue.js frontend
- [django-mqueue-livefeed](https://github.com/synw/django-mqueue-livefeed): live application events feed

#### Utilities

- [ipython](http://ipython.org/) : powerfull python shell integrated with Django
- [django-compressor](https://github.com/django-compressor/django-compressor): to compress static assets
- [django-reversion](https://github.com/etianen/django-reversion) for version control
- [django-mptt](https://github.com/django-mptt/django-mptt): utility for working with trees
- [django-braces](https://github.com/brack3t/django-braces): usefull mixins
- [django-extensions](https://github.com/django-extensions/django-extensions) : usefull tools
- [django-mqueue](https://github.com/synw/django-mqueue): for logging app events 
- [django-filebrowser-no-grappelli](https://github.com/smacker/django-filebrowser-no-grappelli): files management
- [django-dirtyedit](https://github.com/synw/django-dirtyedit): edit files in the admin interface

#### Bootstrap stuff

- [django-bootstrap-form](https://github.com/tzangms/django-bootstrap-form)
- [django-bootstrap3](https://github.com/dyve/django-bootstrap3)

#### Developement (opional)

- [django-debug-toolbar](https://github.com/django-debug-toolbar/django-debug-toolbar) for apps debug
- [pytest-django](https://github.com/pytest-dev/pytest-django): test suite
- [pytest-cov](https://github.com/pytest-dev/pytest-cov): coverage for pytest
- [coverage](https://bitbucket.org/ned/coveragepy): utility for test coverage reporting
- [django-autofixture](https://github.com/gregmuellegger/django-autofixture): for generating test data

#### Templates

Batteries are included with a base template set

## Todo

- [ ] Kick out Bootstrap and Jquery
- [ ] Flex templates
- [x] Better installer for realtime modules
