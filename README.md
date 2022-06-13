# Django demo project

# How to run project.
1. Clone the project repository.
    - Add .env configuration file
2. Create virtual environment with name env.
    - Example is "virtualenv env"
3. Activate the virtual environment.
    - Example is "source env/bin/activate" For MAC and Linux os   
    - Example is "source env/Scripts/activate.psl" For Windows os   
4. Install all th dependencies from requirements.txt file.
    - Example is "pip install -r requirements.txt"
5. Set the databse configuration in settings.py file on DATABASES section.
6. Create all migrations in databse.
    - 1 python manage.py makemigrations
    - 2 python manage.py migrate
7. Run your project.
    - Example is "python manage.py runserver"
