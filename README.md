# giddy-shortner
The application is python and flask based

Install phython (Python 3 advised). Download from here https://www.python.org/downloads/

Download the url shortner application from github - https://github.com/goluniran/giddy-shortner.git

Extract the files in the downloaded zip file into a folder (named core) created in your home directory.

Ensure the 'core' folder is added to the sys.path of your windows device.
(see: https://www.youtube.com/watch?v=gb9e3m98avk)

Open a terminal (or  the windows command (cmd) prompt) and run the following codes to install dependencies within the pipenv virtual environment 

%pip install pipenv

%pipenv shell

%pipenv install Flask

%pipenv install Flask-Migrate

%pipenv install Flask-SQLAlchemy

%pipenv install psycopg2

%pipenv install gunicorn

%pipenv install python-decouple


Export the FLASK_APP environment variable
%set FLASK_AP=main


Initialise and migrate database
%flask db init — to initialize the database at the beginning (used only once)

%flask db migrate — to migrate the new changes to the database (used every time we make changes in the database tables)

%flask db upgrade - used with the migrate command to upgrade the database with new changes


Run the flask url shortening app server
%flask run

Accessing the user inteface 
Done via a browser on http://127.0.0.1:5000/ 

strictly GUI based app launch available soon!
