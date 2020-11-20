# Strapi application

A quick description of your strapi application

## Curso
- https://www.udemy.com/course/react-avancado/learn/lecture/21076716#overview
- https://www.udemy.com/course/criando-um-ambiente-de-desenvolvimento-no-windows/learn/lecture/17962942#overview
## FAQ
- https://github.com/react-Avancado/faq

## Commands
- yarn create strapi-app app

## DB POSTGRES
- sudo service postgresql start
- sudo service postgresql status

## Popular PG (aula 56):
- psql -h 127.0.0.1 -U strapi -d strapi -W < strapi.sql
## Backup PG:
- pg_dump -c --if-exists --exclude-table=strapi_administrator -h 127.0.0.1 -U strapi -d strapi -W > strapi_new.sql


## MISC
- https://strapi.io/documentation/v3.x/guides/registering-a-field-in-admin.html#setup

