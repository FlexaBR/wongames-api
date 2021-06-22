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

ir para outro database:
\c wongames

listar tabelas de dentro do db (wongames):
\dt

listar dados da tabela (não esquecer ; no final)
SELECT * FROM mytable;
para tabelas com - no nome. Ex: users-permissions_user
utilizar entre ""
SELECT * FROM "users-permissions_user";

Zerar a tabela (apagar dados):
TRUNCATE "users-permissions_user";


AQUI BIZU:
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04-pt

https://www.datacamp.com/community/tutorials/10-command-line-utilities-postgresql?utm_source=adwords_ppc&utm_campaignid=1455363063&utm_adgroupid=65083631748&utm_device=c&utm_keyword=&utm_matchtype=b&utm_network=g&utm_adpostion=&utm_creative=332602034358&utm_targetid=dsa-429603003980&utm_loc_interest_ms=&utm_loc_physical_ms=1031654&gclid=CjwKCAjwgOGCBhAlEiwA7FUXkkINGVu6RrRjSYc5LnsEPAX3NnG6iP-zVQ0rA4_-hcgbGvffOEcIqRoC3CEQAvD_BwE


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
- yarn add @ckeditor/ckeditor5-react @ckeditor/ckeditor5-build-cl


npm install -g maildev
