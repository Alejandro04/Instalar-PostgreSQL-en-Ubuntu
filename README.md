# Instalar PostgreSQL en Ubuntu 

## Instalar PostgreSQL 

~~~bash
sudo apt-get -y install postgresql postgresql-contrib
~~~

Ingrese a PostgreSQL con el siguiente comando 
~~~bash
sudo su - postgres

psql
~~~

Crea el usuario y la contraseña para administrar bases de datos  con PostgreSQL. 

~~~bash
create user alejo with password '123456';
~~~

Dar permisos de super usuario a `alejodev`.
~~~bash
alter user alejo with superuser;
~~~

## Crear base de datos con PostgreSQL 
Podemos crear nuestro primer base de datos con el siguiente comando para el usuario `alejodev`. 

~~~bash
create database some_api owner alejodev; 
~~~ 

Listar base de datos. 
~~~bash
\l

\list
~~~

Para salir
~~~bash
exit
~~~

## Ejecutar PgAdmin4 
Buscas en tus aplicaciónes logo de PgAdmin o PotgreSQL, luego colocas los credenciales. a `Add New Server`,  

- En general agregamos el nombre de sevidor. 
- En Connection Host `localhost`  el puerto por defecto. 
- En Username `alejodev` y `password`
