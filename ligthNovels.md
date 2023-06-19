# Ligth Novels

## Listado de Entidades

### novelas_ligeras

- novela_id: Id Novela Ligera **(PK)**
- nombre: Nombre
- tipo_genero: Genero **(FK)**
- estado: Estado **(FK)**
- publicacion: Fecha de Publicacion
- volumenes_publicados: Volumenes Publicados
- idioma: Lenguaje **(FK)**

### tipo_genero

- genero_id: Id Genero **(PK)**
- tipo_genero: Clase de Genero

### estado

- estado_id: Id Estado **(PK)**
- estado: Estado

### idioma

- idioma_id: Id Lenguaje **(PK)**
- idioma: Lenguaje
