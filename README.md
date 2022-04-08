# message_board
This is a complete django project for message_board app.It can able to manage cms service.cms state for Content Management System. Basically, It is a software application or a set of programs that are used to create and manage digital content. It provides capabilities for multiple users with different permission levels to manage web pages.Eventually, some testing scanerio has been done for this application.

* Create a virtual Environment for python

      python -m venv py-env/message_board

* Activate the virtual environment

      .\py-env\message_board\Scripts\activate

* Upgrade the version of python

      pip install --upgrade pip

* Install django and use the version 4.0.0

      pip install django

      python -m pip install django~=4.0.0

* Update django

      python -m pip install --upgrade pip

* Create project level project

      django-admin startproject message_board .

* Make migration when you update your model

      python manage.py makemigrations

      python manage.py migrate

* Run the project


      python manage.py runserver

* Create an app level project

      python manage.py startapp posts

* Which records an environment's current package list into requirements. txt

      pip freeze > requirements.txt

* Which install the required dependencies of python.

      pip install -f requirements.txt

* After creating some model the project needs to migrate the date in sqlite database.

Note: that you don’t have to include a name after makemigrations. If you simply run python manage.py makemigrations, a migrations file will be created for all available changes throughout the Django project. That is fine in a small project such as the message_board app with only a single app, but most Django projects have more than one app! Therefore ,if you made model changes in multiple apps the resulting migrations file would include all those changes! This is not ideal. Migrations file should be as small and concise as possible as this makes it easier to debug in the future or even roll back changes as needed. Therefore, as a best practice, adopt the habit of always including the name of an app when executing the makemigrations command!

        python manage.py makemigrations posts

        python manage.py migrate


* Django was originally built as a newspaper CMS (Content Management System). The idea was that journalists could write and edit their stories in the admin without needing to touch “code.” Over time, the built-in admin app has evolved into a fantastic, out-of-the-box tool for managing all aspects of a Django project.
Django Admin : http://127.0.0.1:8000/admin/


         python manage.py createsuperuser

* Test the test date in django project

      python manage.py test

* Deployment in heroku (Tutorial )
      https://realpython.com/django-hosting-on-heroku/
