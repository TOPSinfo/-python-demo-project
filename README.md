# User Authentication System

## Users Types
1. Super Admin
2. Staff User
3. Guest User

## Project Description
This is **User Authentication System** which allows users to Register and Login
in the system.

**Super Admin** can manage whole project. Super Admin can create users, edit users, and delete 
users. Super Admin can also Activate/Deactivate users. Super Admin can also give permissions
to the users like  Create User, Change User, Delete User, and View User. Super Admin can
also filter users based on their status like PENDING, APPROVED, or REJECTED.

**Staff User** can Create User, Change User, and Delete User according to their permissions.
Staff User can also Update their profile. Staff User can also Register in to this system.

**Guest User** can Register, Login, Update their profile, and Logout from system.


## Project Functionalities
1. Register User (Staff and Guest User)
2. Login into the system (Staff and Guest User)
3. Change User Profile (Staff and Guest User)
4. Create User (Staff User)
5. Edit User (Staff User)
6. Delete User (Staff User)
7. Forget Password (Staff and Guest User)
8. User Permissions (Super Admin)


## Steps to run project.
1. Clone the project repository.

    ```git clone "https://git.topsdemo.in/nimesh/python-demo-project.git"```

2. Add .env configuration file

    ```
    EMAIL_HOST_USER=<YOUR EMAIL ID>
    EMAIL_HOST_PASSWORD=<YOUR EMAIL ACCOUNT APP PASSWORD>
    ```

3. Create virtual environment with folder name env. Execeute bellow command to create virtual environment.

    ```virtualenv env```

4. Activate the virtual environment.

    **For MAC and Linux :-**
        ```source env/bin/activate```  
    **For Windows os:-**
        ```source env/Scripts/activate.psl```

5. Install all the dependencies from requirements.txt file.

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
    - Make sure you have install any of these above databses in your system.

7. Create all migrations in databse.

    ```
    python manage.py makemigrations
    python manage.py migrate
    ```

8. Run your project.

    ```python manage.py runserver```
