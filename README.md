# Django-Basic-Commands

### 1. Create a Django project

To create the initial Django project structure, open your OS terminal and cd to the directory or folder where you want to keep your Django project code. Then run the following command on the chosen terminal which will create a directory/folder with the <project_name> provided in the command within the present working directory.

```
$ django-admin startproject <project_name>
```

### 2. Make migrations command

To convert the Python code written for the model classes (which further represents tables in the database) into database queries. And it becomes necessary to run this command whenever we make any kind of changes to our database class models. To run the following command move inside the project’s folder which contains the manage.py file which will create the necessary database files inside the main project directory.
```
$ python3 manage.py makemigrations
```

### 3. Migrate Command

We need to run this command to create tables in the specified database based on the defined Python class models. This command is responsible for applying or un-applying migrations. When we run this command for the first time all migrations related to the default apps (provided by the Django framework) are applied.
```
$ python3 manage.py migrate
```

### 4. Collect static files

In Django, we deal with the static files differently. It is advisable to create a separate folder and keep all the static files there. We need these Django commands to make it aware of the static files present inside the main project directory.
```
$ python3 manage.py collectstatic 
```

### 5. Create a Django App

A Django project is a collection of apps and configurations for a website. A project can have multiple apps inside it and an app can be included in several Django projects. This command is required to create a Django app inside the Django project which will generate the basic directory structure of a Django app.
```
$ python3 manage.py startapp <app_name>
```

### 6. Create a superuser

It is an essential and necessary command to log in to the default admin interface panel provided by the Django framework. This command is required to create a superuser for the Admin interface who has the username, password, and all other necessary permissions to access and manage the Django website.
```
$ python3 manage.py createsuperuser
```

### 7. Change the password

There are chances, we forget our password of the default admin interface panel. Then it becomes very much necessary to reset it because without a password we will not be able to get access to the default admin interface pannel. We must provide the appropriate <username> whose password has to be reset while running this command.
```
$ python3 manage.py changepassword <username>
```
### 8. Run server

We need this command to verify and test our Django apps and websites by running them on the local server. By default, this command runs the Django development server on the internal IP at port number 8000. If we want, we can also change the development server’s IP and port number by sending them as command-line arguments.
```
$ python3 manage.py runserver 
```
