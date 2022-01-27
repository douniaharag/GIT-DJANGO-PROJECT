### Creating a Blog Application using Django

Installing Django In The Virtual Environment
If you have already installed Django, you can skip this section and jump straight to the Setting up the project section. To Install Django on your virtual environment run the below command

```
pip <span class="hljs-keyword">install</span> Django
```

This will install the latest version of Django in our virtual environment. To know more about Django installation read: How To Install Django


### Setting Up The Project
In your workspace create a directory called mysite and navigate into it.

```
cd Desktop
mkdir mysite
cd mysite
```

Now run the following command in your shell to create a Django project.

```
django-admin startproject mysite
```

This will generate a project structure with several directories and python scripts.

Navigate into the outer directory where manage.py script exists and run the below command.

```
cd mysite
python manage.py startapp blog
```

Next, make migrations.

```
python manage.py migrate
```

This will apply all the unapplied migrations on the SQLite database which comes along with the Django installation.

Let’s test our configurations by running the  Django’s built-in development server.

```
python manage.py runserver
```

Open your browser and go to this address ```http://127.0.0.1:8000/``` if everything went well you should see this page.
