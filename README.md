# User Authentication System

## Users Types
1. Super Admin
2. Staff User
3. Gest User

## Project Description
This is **User Authentication System** which allows users to Register and Login
in the system.

**Super Admin** can manage whole project they can create users, edit users, and delete 
users. Super Admin can also Active/Deactivate users. Super Admin can also give permissions
to the users like  Create User, Change User, Delete User, and View User. Super Admin can
also filter users based on their status like PENDING, APPROVED, or REJECTED.

**Staff User** can Create User, Change User, and Delete User according to their permissions.
Staff User can also Update their profile. Staff User can also Register.

**Gest User** can Register, Login, Update their profile, and Logout.


## Project Functionality
1. Register User (Staff and Gest User)
2. Login into the system (Staff and Gest User)
3. Change User Profile (Staff and Gest User)
4. Create User (Staff User)
5. Edit User (Staff User)
6. Delete User (Staff User)
7. Forgot Password (Staff and Gest User)
8. User Permissions (Super Admin)


## Steps to run project.
1. Clone the project repository.

    ```git clone "https://git.topsdemo.in/nimesh/python-demo-project.git"```

2. Add .env configuration file

    ```
    EMAIL_HOST_USER=dhruvil.m.panchal@gmail.com
    EMAIL_HOST_PASSWORD=wvraxwzgczxofoqy
    ```

3. Create virtual environment with folder name env. Execeute bellow command

    ```virtualenv env```

4. Activate the virtual environment.

    **For MAC and Linux os**
        ```source env/bin/activate```  
    **For Windows os**
        ```source env/Scripts/activate.psl```

5. Install all th dependencies from requirements.txt file.

    ```pip install -r requirements.txt```

6. Set the databse configuration in settings.py file on DATABASES section.

    ```
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql_psycopg2',
            'NAME': 'authsysdb', 
            'USER': 'authsys', 
            'PASSWORD': 'authsys@123',
            'HOST': 'localhost', 
            'PORT': '5432',
        }
    }
    ```

    - Here you can use any databse like sqlite, mysql or postgresql.
    - Make sure you have install any of the above databses in your system.

7. Create all migrations in databse.

    ```python manage.py makemigrations```
    ```python manage.py migrate```

8. Run your project.

    ```python manage.py runserver```
