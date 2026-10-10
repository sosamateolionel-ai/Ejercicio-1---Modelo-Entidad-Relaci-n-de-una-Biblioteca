# Ejercicio 1 - Modelo Entidad-Relación de una Biblioteca

## Descripción

Este ejercicio consiste en diseñar un modelo Entidad-Relación (DER) para un sistema de gestión de biblioteca. El modelo representa los libros, sus autores, los ejemplares disponibles, los usuarios registrados y los préstamos realizados.

## Entidades y atributos

### 1. Libro

Representa los libros registrados en la biblioteca.

* `id_libro`: identificador del libro.
* `titulo`: título del libro.
* `editorial`: editorial que lo publica.
* `edicionAño`: año de edición.

### 2. Autor

Representa a los autores de los libros.

* `id_autor`: identificador del autor.
* `nombre`: nombre del autor.
* `apellido`: apellido del autor.
* `dni`: documento de identidad.

### 3. Libro_Autor

Representa la relación entre los libros y sus autores.

* `id_autor`: identificador del autor.
* `id_libro`: identificador del libro.

### 4. Ejemplar

Representa cada copia física de un libro disponible en la biblioteca.

### 5. Usuario

Representa a las personas que utilizan los servicios de la biblioteca.

* `id_usuario`: identificador del usuario.
* `nombre`: nombre del usuario.
* `apellido`: apellido del usuario.
* `dni`: documento de identidad.
* `domicilio`: dirección del usuario.

### 6. Prestamo

Registra los préstamos de ejemplares realizados por los usuarios.

* `id_prestamo`: identificador del préstamo.
* `fecha`: fecha del préstamo.
* `fecha_dev`: fecha de devolución.
* `edicion`: edición asociada.
* `autor`: autor asociado.

## Relaciones y cardinalidades

* **Libro – Autor:** permite asociar libros con sus autores mediante la entidad `Libro_Autor`.
* **Libro – Ejemplar:** un libro puede tener varios ejemplares.
* **Ejemplar – Prestamo:** permite registrar los préstamos de los ejemplares.
* **Usuario – Prestamo:** un usuario puede realizar varios préstamos.

## Objetivo

Representar la estructura de una base de datos para una biblioteca, identificando las entidades, sus atributos y las relaciones necesarias para administrar libros, ejemplares, autores, usuarios y préstamos.


