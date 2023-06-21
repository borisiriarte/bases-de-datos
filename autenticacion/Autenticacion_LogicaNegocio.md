# Sistema de Autenticacion

## Listado de Entidades

### Usuarios **(ED)**

- usuario_id **(PK)**
- username **(UQ)**
- password
- email **(UQ)**
- nombre
- apellido
- avatar
- activo
- fecha_creacion
- fecha_actualizacion

### roles(perfiles) **(EC)**

- rol_id **(PK)**
- nombre_rol
- descripcion

### permisos **(EC)**

- permiso_id
- nombre_permiso
- descripcion

### roles_por_usuario **(EP)**

- rxu_id **(PK)**
- usuario_id **(FK)**
- rol_id **(FK)**

### permisos_por_roles **(EP)**

- pxr_id **(PK)**
- rol_id **(FK)**
- permiso_id **(FK)**

## Relaciones

1. Los **Usuarios** tienen **roles** (_M a M_).
2. Los **Roles** tienen **permisos** (_M a M_).

## Logica de Negocio

### Usuarios

1. Crear usuario
1. Validad un usuario
1. Leer un usuario en especifico
1. Leer todos los usuarios
1. Actualizar un usuario
1. Eliminar un usuario
1. Habilitar un usuario
1. Deshabilitar un usuario
1. Actualizar datos de un usuario
1. Actualizar la contraseña de un usuario

### roles(perfiles)

1. Crear rol
1. Leer un rol en especifico
1. Leer todos los roles
1. Actualizar un rol
1. Eliminar un rol

### permisos

1. Crear permiso
1. Leer un permiso en especifico
1. Leer todos los permisos
1. Actualizar un permiso
1. Eliminar un permiso

### roles_por_usuario

1. Crear un rxu
1. Leer un rxu en especifico
1. Leer todos los rxu
1. Leer todos los rxu de un usuario
1. Eliminar un rxu

### permisos_por_roles

1. Crear un pxr
1. Leer un pxr en especifico
1. Leer todos los pxr
1. Leer todos los pxr de un rol
1. Eliminar un pxr
