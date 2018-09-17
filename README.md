# Palimpsest

A starter template for Django/webpack projects. Features user/team accounts and optional Stripe and Celery integration.

**License: MIT**


## Setting up



## Options
Celery, Stripe, and team accounts are optional. Follow the below steps to get them enabled or disabled.

| Integration   | Yes, I want it | No, remove it |
| ------------- | -------------- | ------------- |
| Stripe        | ??             | ??            |
| Celery        | ??             | ??            |
| Team accounts | ??             | ??            |




## Celery
This app comes with Celery.

To run a celery worker:

```bash
    cd palimpsest
    celery -A palimpsest.taskapp worker -l info
```

Please note: For Celery's import magic to work, it is important *where* the celery commands are run. If you are in the same folder with *manage.py*, you should be right.

