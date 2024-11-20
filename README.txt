Example project for integrating Celery and Redis into a Django application.
Tutorial : 
1- Setup the virtual environment : 
	$ python -m venv venv
	$ source venv/bin/activate
2- Install requirements.txt : 
	$ pip install -r requirements.txt 
3- Generate a secret key and add it in settings.py 
You'll also need to install Redis on your system
Once you have installed all the depencies, you must run this processes at the same time : Django, Redis, Celery
Django : 
	$ python manage.py run server
Redis : 
	$ redis-server
Celery : 
	$ python -m celery -A django_celery worker -l info
Once the three servers are running go to :
http://127.0.0.1:8000/

