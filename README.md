# Consulta #1 Sql

## CONSULTAS SQL


### 1. Para visualizar toda la información que contiene la tabla `usuario` se puede incluir con la instrucción SELECT el caracter `*` o cada una de los campos de la tabla 

- `SELECT * FROM usuario`

![Consulta1](img/tabla_usuario.png "Tabla usuario")

### 2. Seleccionar o visualizar solamente la identificación del usuario.

- `SELECT Identificación FROM usuario`

![Consulta2](img/tabla_identificacion.png "Tabla Identificacion")

### 3. Si se desea obtener los registros cuya identificacion sean mayores o iguales a 150, se debe utilizar la consulta WHERE que especifica las condiciones que deben reunir los registros que se van a seleccionar-

- `SELECT * FROM usuario WHERE identificacion >= 150`

![Consulta3](img/tabla_mayorque.png "Tabla Mayor o igual que")

### 4. Si se desea obtener los registros cuyo sus apellidos sean Vanegas o Cetina, se debe utilizar el operador IN que especifica los registros 
- `SELECT apellidos FROM usuario WHERE apellidos IN ('Vanegas', 'Cetina')`

![Consulta4](img/tabla_apellidos1.png "Tabla Apellidos1")

O se puede utilizar el operador OR.

- `SELECT apellidos FROM usuario WHERE apellidos='Vanegas' OR apellidos='Cetina'`

![Consulta4.1](img/tabla_apellidos2.png "Tabla Apellidos2")

### 5. Si se desea obtener los registros cuya identificacion sea menor de '110' y la ciudad sea 'Cali', se debe utilizar el operador AND.

- `SELECT * FROM usuario WHERE identificacion < 110 AND ciudad_nac='Cali'`

![Consulta5](img/tabla_iden-ciudad.png "Tabla Apellidos2")

### 6. Si se desea obtener los registros cuyos nombres empiecen por la letra 'A', se debe usar el operador LIKE que usa los patrones '%' (todos) y '_' (caracter).

- `SELECT * FROM usuario WHERE nombre LIKE 'A%'`

![Consulta6](img/tabla_nombreA.png "Tabla nombreA")

### 7. Si desea obtener los registros que contengan la letra 'a'.

`SELECT * FROM usuario WHERE nombre LIKE '%a%'`

![Consulta7](img/tabla_nombreconA.png "Tabla nombreConA")

### 8. Si se desea obtener los registros donde la cuarta letra del nombre sea una 'a'.

`SELECT * FROM usuario WHERE nombre LIKE '___a%'`

![Consulta8](img/tabla_nom_4a.png "Tabla nombreConA en cuarto")

### 9. Si se desea obtener los registros cuya identificacion este entre el intervalo 110 y 150, se debe utilizar la clausula BETWEEN, que sirve para especificar un intervalo de valores.

`SELECT * FROM usuario WHERE identificacion BETWEEN '110' AND '150'`

![Consulta9](img/tabla_seleccionar_entre.png "Tabla seleccionar entre x variables")

## COMANDO DELETE

### 10. Para eleminar solamente los registro cuya identificacion sea mayor de 130.

`DELETE FROM usuario WHERE identificacion > '130'`

![Consulta10](img/tabla_delete_usuarios.png "Tabla delete users")

![Consulta10.1](img/tabla_delete_usuarios-1.png "Tabla delete users1")

## COMANDO UPDATE

### 11. Para actualizar la ciudad de nacimiento de Andres Vanegas, cuya informacion es 118.

`UPDATE usuario SET ciudad_nac = 'Manizales' WHERE identificacion='118'`

![Consulta11](img/tabla_actualizar_datos.png "Tabla actializar datos")

## TITULO

### 12. -TEXTO-

![Consulta12](img/tabla_pedidos.png "Tabla Pedidos")


