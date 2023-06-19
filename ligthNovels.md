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

1. Una **novela ligera** _pertenece_ a un **tipo de genero** (_1 a M_)
2. Una **novela ligera** _se encuentra_ en un **estado de publicacion** (_1 a 1_)
3. Una **novela ligera** _es escrita_ en un **idioma** (_1 a 1_)

## Diagramas

### Modelo Entidad-Relacion

### Modelo Entidad-Relacion BD

<!-- ![Modelo Entidad Relacion]() -->

## Reglas de negocio

### novelas_ligeras

1. Crear el registro de las novelas traducidas
2. Leer la informacion de una novela especifica
3. Leer todos los registros de la entidad novelas ligeras
4. Actualizar los datos de la novela
5. Eliminar los datos de una carrera dada una condicion en particular

### tipo_genero

1. Crear el registro de un o unos tipos de generos
2. Leer el registro del tipo o tipos de generos de cada novela
3. Leer todos los registros de la entidad tipo_genero
4. Actualizar los datos de el genero de cada novela
5. Eliminar uno a mas tipos de generos

### estado

1. Crear el registro del estado actual de la novela
2. Leer el registro del estado de la novela
3. Actualizar los datos del estado de la novela
4. Eliminar el registro del estado de la novela

### idioma

1. Crear el registro del idioma al que fue traducida la novela y su idioma original
2. Leer el registro del idoma o idiomas al que fueron traducidos cada novela
3. Leer todos los registros de los idiomas de las novelas
4. Actualizar los datos del idiomas o idiomas de la novela
5. Eliminar uno a mas idiomas
