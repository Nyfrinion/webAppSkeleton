Creating a django project: django-admin startproject django_project
Creating a django app: python manage.py startapp django_app
Creating a react app: npx create-react-app frontend
Docker build: docker-compose up --build
Docker bring down: docker-compose down
Django/Postgresql Migration: docker-compose exec backend python manage.py migrate --noinput
Check for default Django DB tables: docker-compose exec db psql --username=hello_django --dbname=hello_django_dev
Check the volume: docker volume inspect django-on-docker_postgres_data

note to self: to integrate react and django have
django create restful apis? and post via react?

Brief explanation of each relevant file/folder:

backend

    django_app -> generated; app created with django(more details below)
    django_project -> generated; project created with django(more details below)
    static -> created; folder for static content(img, css, etc)
    Dockerfile -> created;
    manage.py -> generated; django managment script; used to create app
    requirement.txt -> python requirements file, info grabbed by dockerfile

frontend

    Dockerfile -> created;
    node_modules -> generated;
    public -> generated;
    src -> generated;
    .gitignore -> generated;
    package-lock.json -> generated;
    package.json -> generated;
    README.md -> generated; markdown file created by react app

other

    docker-compose.yml -> created; YAML file for docker-compose configuration
    README.md -> created; markdown file with instructions/details
    .env -> created; environment variables for docker

