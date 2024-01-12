# In development

## Application builded with Django, React and PostgreSQL

## For local installation

***In the backend directory, create a new vitual environment using venv***

python -m venv venv

***Activate the environment***

source venv/bin/activate

***Install the dependencies that django needs***

pip install -r ../requirements.txt

***In the frontend directory, use the following commands to install the dependencies***

yarn install

***The command bellow will create the folder "build" and copy it to the backend directory***

yarn build

## For dockerized installation

***In the frontend directory, use the following commands to install the dependencies***

yarn install

***The command bellow will create the folder "build" and copy it to the backend directory***

yarn build

***Create the environment variables in a file .env on the root directory***

***Build the images and the containers***

docker compose build && docker compose up -d

***Acess the api container and make all the migrations to the database***

docker compose exec api sh
python manage.py makemigrations
python manage.py migrate

***Still on the api container, create a django superuser to do CRUD operations on the web interface***

python manage.py createsuperuser
