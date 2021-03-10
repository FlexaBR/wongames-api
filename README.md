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

Alterne para a conta postgres no seu servidor digitando:
sudo -i -u postgres
Saia do prompt do Postgres digitando:
exit

Iniciar a sessão diretamente no Postgres sem o shell
sudo -u postgres psql 
Saia do prompt do Postgres digitando:
\q
listar os dbs:
\l


## Popular PG (aula 56):
- psql -h 127.0.0.1 -U strapi -d strapi -W < strapi.sql (outra aula, não usar)
- curl -X POST http://localhost:1337/games/populate (chama o service - para testes colocar console.log no service e rodar o curl)
## Backup PG:
- pg_dump -c --if-exists --exclude-table=strapi_administrator -h 127.0.0.1 -U strapi -d strapi -W > strapi_new.sql


## MISC
- yarn develop --watch-admin

- https://strapi.io/documentation/v3.x/guides/registering-a-field-in-admin.html#setup

## Plugin CKEditor
- https://www.udemy.com/course/react-avancado/learn/lecture/21124004#overview 
- yarn strapi generate:plugin wysiwyg
- cd plugins/wysiwyg
- yarn add @ckeditor/ckeditor5-react @ckeditor/ckeditor5-build-classic


