int= nº1 de integral(xxx) cantidad de bits a almacenar
varchar= cadena de caracteres variables(xxx) cantidad de bits a almacenar
show databases; (muestra la base de datos)
show tables; (muestra las tablas de una base de datos)
where (donde buscar)
use xxx; (bbdd a la que quieres acceder)

describe xxxx; (nombre de la columna a la que acceder)

Select xxx (columna) xxx (columna) from xxxx; (la tabla)



Select xxx (columna) xxx (columna) from xxxx (la tabla) where xxxx (la tabla) = "XX"  (lo que buscas)

-Crear BBDD

create database xxxx; (nombre de la bbdd)

-Crear tabla
create table xxxx(nombre de la tabla)(xxxxx(nomb));

create table users(id int(32), username varchar(32), password varchar(32));


-Insertar datos
insert into users(id, username, password) values(1, "admin", "admin123$!");

insert into "tabla"(columna1, columna2, columna3) value("dato1", "dato2", "dato3")(2, omar, pocholo); 

-Crear usuario
create user "xxx"@"localhost" identified by "password";

-Dar acceso completo a un usuario a una BBDD
grant all privileges on xxxx.*(nombre de la BBDD) to "user"@"l"ocalhost"


_ver los datos de una tabla 
select * from xxxx; (nombre de la tabla)