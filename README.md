# my_ubuntu_cheat_sheet

1. **ModuleNotFoundError: No module named 'distutils.util' Error:**

solution: sudo apt-get install python3.9-distutils

2. **install and using pgadmin:**

[for installation:]
(https://www.pgadmin.org/download/pgadmin-4-apt/)

[insert the row in database:]
(https://stackoverflow.com/questions/22755230/how-to-insert-a-row-in-postgresql-pgadmin)

3. **django currency link:**
(https://www.youtube.com/watch?v=Rk8YTRAnSdI)

4. **change /etc/hosts file:**
(https://askubuntu.com/questions/562310/how-to-edit-read-only-file-in-etc)

5. **upload image and video(file) on heroku:**
(https://www.dothedev.com/blog/heroku-django-store-your-uploaded-media-files-for-free/)

6.**free domain for website:**
(https://www.freenom.com)

7.**deploy css in heroku:**
(https://devcenter.heroku.com/articles/django-assets)

8.**deploy rabbitmq & celery in heroku:**
you just adding rabbitmq to heroku app,
after that you should adding :
CELERY_BROKER_URL = 'amqps://cmtjfjxf:MxPBcqiEZifOJl2aEasLUdUg7104Nsfy@finch.rmq.cloudamqp.com/cmtjfjxf'
to settings.py file
after this you shold adding:
worker: celery -A myshop worker -l info
at Procfile
