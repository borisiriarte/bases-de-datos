# BorisGram

## Listado de Entidades

### posts **(ED)**

- post_id **(PK)**
- post_date
- descripcion
- foto
- user_id **(FK)**

### user **(ED)**

- user_id **(PK)**
- user_date
- user_name
- email **(UQ)**
- password
- telefono **(UQ)**
- biography
- web
- avatar
- birthdate
- gender
- country **(FK)**

### comments **(ED | EP)**

- comment_id **(PK)**
- comment_date
- comment
- post_id **(FK)**
- user_id **(FK)**

### hearts **(ED | EP)**

- heart_id
- heart_date
- post_id **(FK)**
- user_id **(FK)**

### follows **(ED | EP)**

- follow_id **(PK)**
- follow_date
- follow_user **(FK)**
- user_id **(FK)**

### countries **(EC)**

- country_id
- country_name

## Relaciones

1. Los **Users** publican **post** (_1 a M_).
1. Los **Users** hacen **comments** (_1 a M_).
1. Los **Users** dan **hearts** (_1 a 1_).
1. Los **Users** dan **follows** (_1 a M_).
1. Los **Users** tienen **follows** (_1 a M_).
1. Los **Users** pertencen **country** (_1 a 1_).
1. Los **Post** tienen **comments** (_1 a M_).
1. Los **Post** tienen **hearts** (_1 a M_).

## Logica de Negocio

### posts

1. Crear un post.
1. Leer todos los posts.
1. Leer un post en particular.
1. Leer los post de un user.
1. Actualizar el plot de un post.
1. Eliminar un post.

### users

1. Crear un user.
1. Leer todos los users.
1. Leer un user en particular.
1. Validar un user.
1. Actualizar datos del user.
1. Actualizar password de user.
1. Eliminar user.

### comments

1. Crear un comment en un post.
1. Leer todos los comments de un post.
1. Leer un comment de un post.
1. Contar el número de comments de un post.
1. Eliminar comment en un post.

### hearts

1. Crear heart de user en un post.
1. Contar el número de hearts de un post.
1. Eliminar heart de user en un post.

### follows

1. Crear follow de un user.
1. Contar el número de followers de un user.
1. Contar el número de followings de un user.
1. Eliminar follow de un user.

### countries

1. Crear country.
1. Leer todos los countries.
1. Leer un country.
1. Actualizar un country.
1. Eliminar country.
