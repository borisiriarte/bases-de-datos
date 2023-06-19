# Ligth Novels

## Listado de Entidades

### novelas_ligeras **(ED)**

- novela_id: Id Novela Ligera **(PK)**
- nombre: Nombre
- tipo_genero: Genero **(FK)**
- estado: Estado **(FK)**
- publicacion: Fecha de Publicacion
- volumenes_publicados: Volumenes Publicados
- idioma: Lenguaje **(FK)**

### tipo_genero **(EC)**

- genero_id: Id Genero **(PK)**
- tipo_genero: Clase de Genero

### estado **(EC)**

- estado_id: Id Estado **(PK)**
- estado: Estado

### idioma **(EC)**

- idioma_id: Id Lenguaje **(PK)**
- idioma: Lenguaje

## Relaciones

1. Una **novela ligera** _pertenece_ a un **tipo de genero**
2. Una **novela ligera** _se encuentra_ en un **estado de publicacion**
