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

8.**deploy rabbitmq & celery in heroku:**<br>
<pre>
you just adding rabbitmq to heroku app,
after that you should adding :
CELERY_BROKER_URL = 'xxxxxxxxxxxxx'
to settings.py file
after this you shold adding:
worker: celery -A myshop worker -l info
at Procfile
</pre>

# DRF:<br>
1.**djang documentation:**<br>
<pre>
  1.(https://drf-yasg.readthedocs.io/en/stable/readme.html)
  2.change drf_yasg to drf_yasg2
  3.[https://stackoverflow.com/questions/55007336/drf-yasg-customizing?rq=1]</pre>
<br>
  
# Fastapi:<br>
1.**upload image in fastapi:**<br>
  <pre>
  For uploading image wee need 3 step:
    1.install cloudinary
    2.import:
      import cloudinary
      import cloudinary.uploader
    3.configure cloudinary:
        cloudinary.config( 
          cloud_name = "XXXXXXXXXXXXXX", 
          api_key = "XXXXXXXXXXXXXXXXX", 
          api_secret = "XXXXXXXXXXXXXXXXX" 
        )
    4.adding function like this:
        @app.post("/uploadfile/")
        async def create_upload_file(file: UploadFile = File(...)):
          filename = file.filename
          result =cloudinary.uploader.upload(file.file)
          url = result.get("url");
          return url
  </pre>
  
 Or We can use bellow url<br>
 (https://github.com/tiangolo/fastapi/issues/426)

2.**setting PostgreSQL:**<br>
(https://youtu.be/CB1J2LUX1WI)


# Ubuntu issue:<br>
1.**chrome proxy does't work:**<br>
(https://askubuntu.com/questions/513840/google-chrome-proxy-settings)


# Heroku:<br>
1.**heroku redis deploying:**<br>
 We can use bellow url<br>
 (https://devcenter.heroku.com/articles/heroku-redis)
