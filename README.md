# Consustal_SQL
Introduccion a SQL

## Base de datos: Ventas
## Tablas: Clientes

#####


## Instrucción SELECT
- Permiteseseclaccionar datos de una tabla.
- Su formato es 

### Consulta N°.1
1. Para visualizar toda la informacion que todo la tabla de Clientes se puede concluir con uno de los campos de la tabla.

- 'SELECT *FROM Cliente´
- 'SELECT identificación, nombre, apellidos, dirreccion, telefono,ciudad_nac,fecha nac FROM Cliente'

![consulta_1](2_oct.png 'consulta_1)!

### Consulta N°.2

2. Para visualizar solamente la indentificacion de Cliente: 'SELECT indentifficación FROM Cliente'

![consulta_2](consulta-2 'consulta_2)!
### Consulta N°3

3. Si se desea obtener los registro mayor o igual  a 150, se debe utilizar la cláusula 'WHERE' que especifica las condiciones que se deban seleccionar : 'SELECT * FROM cLIENTES WHERE indentificacion=150'

![consulta_3](consulta-3 'consulta_3)!

### Consulta N°4

4. Se desea obtener los registris cuyo apellidos sean vagegas o cetina, se debe utulizar el operador  'IN' que especificael refistro que se debe especificae e los registros de la tabla.

'SELECT apellidos, nombre, FORM Cliente M-ERE apellidos, - "vegas" OR apellidos - "Cetina"

[consulta_4](consulta-4 'consulta_4)!

### Consulta N°5

5. Se desea obtener los registros menor a 110 y la ciudad sea cali, se debe usar el operador 'AND' 'SELEC *fORM Cliente WHERE indentificaciom <=110 AND ciudad - 'Cali''

[consulta_5](consulta-5 'consulta_5)!