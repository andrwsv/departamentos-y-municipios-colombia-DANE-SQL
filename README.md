Departamentos y municipios de Colombia en SQL - 2023
Este repocsitorio contiene dos archivos SQL con los departamentos y municipios de Colombia.

Tomado del DANE: Codificación de la División Político Administrativa de Colombia - DIVIPOLA Agosto 2023

#Información de la tablas Tabla departamentos:

[id_departamento - int(2)] => Los IDs de esta tabla corresponden al código de cada departamento asignado por el DANE, por lo que no son consecutivos.
[departamento - varchar(255)]
Tabla municipios:

[id_municipio - int(6)]
[municipio - varchar(255)]
[estado - int(1)] => Campo que su puede emplear para valiadar si el municipio está activo o por alguna razón ya no existe.
[departamento_id - int(2)] => Llave foránea para la relación con la tabla departamentos.
El campo departamento_id está indexado para optimización de las consultas.
[codigo_departamento varchar(5)] =>codigo DANE de 5 caracteres
[Tipo - varchar(100)] => Tipo: Municipio / Isla / Área no municipalizada
[latitud - varchar(100)]
[longitud - varchar(100)] ubicaciones actualizadas de los municipios en el mapa


#Para las dos tablas:

Charset: UTF8MB4
Tipo de almacenamiento: InnoDB
#Sobre los datos

Los datos fueron tomados de la información estadística del DANE año 2023
Scripts generados por Sequel Pro.
