# Palimpsest

A starter template for Django/webpack projects based on [Cookiecutter Django](https://github.com/pydanny/cookiecutter-django). Features user/team accounts and optional Stripe and Celery integration.

**License: MIT**

## Features

* Django 2.1
* Works with Python 3.6
* Renders Django projects with 100% starting test coverage
* Twitter Bootstrap v4.1.1
* 12-Factor based settings via django-environ
* Secure by default
* Optimized development and production settings
* Registration via django-allauth


## Setting up

1) Clone this repository: `git clone https://github.com/lucaluca/palimpsest`
1) Init your repository: `git init`
1) Do a case-sensitive, project-wide replace of "palimpsest" for the name of your app. Rename the `palimpsest` folder to the name of your app.
1) Copy `config/.envs/local` into `.env` in the app folder and generate a secret key and admin site URL
2) If you want Stripe integration, run the steps under **Enable Stripe** below. If you don't, run the steps under **Disable Stripe**.
3) Same for Celery: **Enable Celery** or **Disable Celery**.
4) Same for team accounts: **Enable Team Accounts** or **Disable Team Accounts**.
1) Go [here](https://realfavicongenerator.net/) and upload an image to create favicon files.
  * Drop the generated HTML into the specified section of `base.html`.
  * Put the files in `palimpsest/static/images/favicons/`.


## Options
Celery, Stripe, and team accounts are optional. Follow the below steps to get them enabled or disabled.

### Enable Stripe

### Disable Stripe

### Enable Celery


To run a celery worker:

```bash
    cd palimpsest
    celery -A palimpsest.taskapp worker -l info
```

Please note: For Celery's import magic to work, it is important *where* the celery commands are run. If you are in the same folder with *manage.py*, you should be right.

### Disable Celery

### Enable Team Accounts

### Disable Team Accounts

