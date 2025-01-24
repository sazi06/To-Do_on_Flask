# Flask-Todolist

Flask-Todolist is a simple To Do List web application with the most basic
features of most web apps, i.e. accounts/login, API and (somewhat) interactive
UI.

---
CSS | [Skeleton](http://getskeleton.com/)
JS  | [jQuery](https://jquery.com/)

I've also build a quite similar app in Django:
https://github.com/sazi06/django-todolist


## Explore
Try it out!

To run it directly on your local machine, I suggest using
[venv](https://docs.python.org/3/library/venv.html).

    pip install -r requirements.txt
    FLASK_APP=todolist.py flask run

To add some 'play' data you can run

    pip install -r test-requirements.txt
    flask fill-db

Now you can browse the API:
http://localhost:5000/api/users

Pick a user, login as the user. Default password after `fill-db` is
*correcthorsebatterystaple*.
Click around, there is not too much, but I like the overview under:
http://localhost:5000/todolists
(You must be logged in to see it.)


## Extensions
In the process of this project I used a couple of extensions.

Usage               | Flask-Extension
------------------- | -----------------------
Model & ORM         | [Flask-SQLAlchemy](http://flask-sqlalchemy.pocoo.org/latest/)
Migration           | [Flaks-Migrate](http://flask-migrate.readthedocs.io/en/latest/)
Forms               | [Flask-WTF](https://flask-wtf.readthedocs.org/en/latest/)
Login               | [Flask-Login](https://flask-login.readthedocs.org/en/latest/)
Testing             | [Flask-Testing](https://pythonhosted.org/Flask-Testing/)
