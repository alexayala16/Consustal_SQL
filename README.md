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