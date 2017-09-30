# django-restful
Starting RESTful API w Django
# run the following from your terminal / shell

#create project directory 

mkdir tutorial 
cd tutorial 

# create virtual env 
virtual env 
source env/bin/activate 

#install django and rest framework 
pip install django 
pip install djangorestframework 

#setup new project w single application 
django-admin.py startproject tutorial 
cd tutorial 
django-admin.py startapp quickstart


#sync database for first time 
python manage.py migrate 

#create initial user admin & password 
python manage.py createsuperuser 
# username: admin 
# password: password123

#now add serializers ... go to /tutorial/quickstart and add file called serializers.py
#now add views ... open /tutorial/quickstart/views.py
# next wire up API URLs /tutorials/url.py
# settings - enable pagination and API only accessible to admin users 
# go to /tutorial/settings.py and edit file 
