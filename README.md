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
yarn build

## For dockerized installation

***Create the environment variables in a file .env***

***Build the images and the containers***

docker compose build && docker compose up -d
