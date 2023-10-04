# Consusta_SQL
Introduccion a SQL

## Base de datos: Ventas
## Tablas: Clientes

-Nota: Los pantallasos son rob ados de usted profe por que no tenia tabla por el cambio de equipos PC.
## Instrucción SELECT
- Permiteseseclaccionar datos de una tabla.
- Su formato es 

### Consulta N°1

1. Para visualizar toda la informacion que todo la tabla de Clientes se puede concluir con uno de los campos de la tabla.

- 'SELECT *FROM Cliente´
- 'SELECT identificación, nombre, apellidos, dirreccion, telefono,ciudad_nac,fecha nac FROM Cliente'

![Consulta 1](IMGs/Consulta1.png "consulta_1")

### Consulta N°2

2. Para visualizar solamente la indentificacion de Cliente: 'SELECT indentifficación FROM Cliente'

![Consulta 2](IMGs/Consulta2.png "consulta_2")
### Consulta N°3

3. Si se desea obtener los registro mayor o igual  a 150, se debe utilizar la cláusula 'WHERE' que especifica las condiciones que se deban seleccionar : 'SELECT * FROM cLIENTES WHERE indentificacion=150'

![Consulta 3](IMGs/Consulta3.png "consulta_3")

### Consulta N°4

4. Se desea obtener los registris cuyo apellidos sean vagegas o cetina, se debe utulizar el operador  'IN' que especificael refistro que se debe especificae e los registros de la tabla.

'SELECT apellidos, nombre, FORM Cliente M-ERE apellidos, - "vegas" OR apellidos - "Cetina"

![Consulta 4](IMGs/Consulta4.png "consulta_4")

### Consulta N°5

5. Se desea obtener los registros menor a 110 y la ciudad sea cali, se debe usar el operador 'AND' 'SELEC *fORM Cliente WHERE indentificaciom <=110 AND ciudad - 'Cali''

![Consulta 5](IMGs/Consulta5.png "consulta_5")

### Consulta N°6

6. Si se desea obterner los registros segun el nsegun la letra "A" se usa el operador 'LIKE' que utiliza los patrones.

'SELEC *FROM Cliente Where nombre LIKE'

![Consulta 6](IMGs/Consulta6.png "consulta_6")

### Consulta N°7

7. Se deseaa que los registros que tengan cuyos nombres tengan la letra 'a' 

'SELECT * FROM Cliente WHERE nombre LIKE '%a%''

![Consulta 7](IMGs/Consulta7.png "consulta_7")

### Consulta N°8

8. Se desea obtener los registros donde la cuarta letra  del nombre es 'a'

'SELECT * FROM Cliente Where nombre LIKE '___a''

![Consulta 8](IMGs/Consulta8.png "consulta_8")


### Consulta N°9

9. SI se desea obtener los registros cuya identificacion este entre los intervalos 110 y 150, se debe utilizar la cláusula 'BETWEEN', que sirve para especificar un intervalo de valores.

'SELECT * From Cliente WHERE indentificacion 'BETWEEN 110 AND 150'

![Consulta 9](IMGs/Consulta9.png "consulta_9")

## Instrucción DELETE

- Permite borrar todos o un grupo específico de registros de una tabla.
- Su formato 'DELETE FROM nombre tabla'

### Eliminación N°1

1. Eliminar los registros cuya identificación  > 170.

'DELETE FROM Cliente WHERE indentificacion > 170'

![Eliminación 1](IMGs/Eliminación1.png "Eliminacion_1")

### Eleminación N°2

2. Eliminar los registros cuya indentificación sea igual a 116.

'DELETE FROM Cliente WHERE indentificación = 116'

## Instrucción UPDATE

- Permite actualizar un campo de una tabla.
- Su formato 'UPDATE nombre tabla SET nombre_campo = valor'

### Actualización N°1

1. Para actualizar la ciudad de nacimiento de Cristian Vanegas, cuya indentificación  es 114.

'UPDATE Cliente SET ciudad_nac = 'pereida' WHERE  indentificación=114'

![Actuslización](IMGs/Actualización.png "Actualización")

## Creación tabla Pedido
### Diccionario de datos
|Campo|Tipo de dato|Longitud|
|-----|------------|--------|
|***no_pedido***|varchar|15|
|iden_Cliente|varchar|15|
|fecha_conpra|date||
|fecha_vencimiento|date||
|observacion|varchar|30|

### Modelo Entidad-Relación

![Modelo](IMGs/Modelo.png "Modelo")

## Operador INNER JOIN

- Permite obtener datos de dos o más tablas.
- Cuando se realiza la concatenación de las tablas, no necesariamente se deben mostrar todos los datos de la tabla.
-Su formato es:
'SELECT tabla1.campo, tabla2.campo,...FROM tabla_principal INNER JOIN tabla_secundaria ON campo_comun_tabla1 = campo_comun_tabla2'

1. Para visualizar los campos indentificación,nombre, apellidos de la tabla cliente y N°_pedido, fecha_compra, fecha_vencimiento y observación de la tabla Pedido, se debe realizar la siguiente instrucción:

'SELECT Cliente.Indentificación, Cliente.Nombres, Cliente.Apellidos, Pedido.no_pedido, Pedido.Fecha_vencimiento, Pedido.Observación FROM Cliente INNER JOIN Pedido ON Cliente.Indentificación =Pedido.Ide_cliente'

![Inner join 1](IMGs/Inner_join_1.png "Inner join 1")

2. Para visualizar todos los campos de las tablas Cliente y Pedido donde indentificación sea mayor que 100, se debe revisar la siguiente instrucción:

'SELECT Cliente.*, Pedido.* FROM Cliente INNER JOIN Pedido ON Cliente.identificación = Pedido.iden_Cliente Where Cliente.identificación>100'

![Inner join 1](IMGs/Inner_join_2.png "Inner join 1")