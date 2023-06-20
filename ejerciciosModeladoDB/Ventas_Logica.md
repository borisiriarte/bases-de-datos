# Ventas

## Listado de entidades

### Clientes **(ED)**

- cliente_id **(PK)**
- nombres
- apellidos
- telefono **(UQ)**
- email **(UQ)**
- direccion
- cp
- ciudad
- pais **(FK)**

### Productos **(ED)**

- producto_id **(PK)**
- nombre
- descripcion
- fotografia
- precio
- cantidad

### Ventas

- venta_id **(PK)**
- cliente_id
- fecha
- monto

### articulos_x_venta **(EP)**

- articulo_id **(PK)**
- venta_id **(FK)**
- producto_id **(FK)**
- cantidad

### paises **(EC)**

- pais_id
- nombre
- dominio **(UQ)**

## Relaciones

1. Un **cliente** tiene **pais** (_1 a 1_).
2. Un **cliente** genera **venta** (_1 a M_).
3. Un **venta** tiene **articulos** (_1 a M_).
4. Un **articulo** es un **producto** (_1 a 1_).
