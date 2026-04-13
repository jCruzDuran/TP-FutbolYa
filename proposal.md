# Propuesta TP DSW

## Grupo
### Integrantes
* 47133 - Durán, Juan Cruz.
* 42101 - Gomez, Fernando.
* 52938 - Faccio, Juan Ignacio.

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema: SportAll
### Descripción
*Aplicación para reservar espacios en un complejo deportivo para distintos tipo de actividades*

### Modelo
<img width="1382" height="971" alt="image" src="https://github.com/user-attachments/assets/a0c75106-0c34-4715-967e-c4e36ac583a0" />

Link con la imagen del modelo de dominio: https://drive.google.com/file/d/1gXwBSWCO8L0tnm3WbJGHOtN9KUj2y0FZ/view?usp=sharing

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuarios<br>2. CRUD Tipos de Cancha<br>3. CRUD Tipos de Evento|
|CRUD dependiente|1. CRUD Cancha {depende de} CRUD Tipo Cancha<br>2. CRUD Reserva {depende de} CRUD Usuario|
|Listado<br>+<br>detalle| 1. Listado de reservas, con fecha de reserva, hora inicio, hora fin, usuario, numero de cancha => detalle CRUD Reserva<br> 2. Listado de canchas disponibles filtrado por rango de fecha, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente|
|CUU/Epic|1. Reservar una cancha<br>2. Realizar el check-in de una reserva|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Habitacion<br>2. CRUD Servicio<br>3. CRUD Localidad<br>4. CRUD Provincia<br>5. CRUD Habitación<br>6. CRUD Empleado<br>7. CRUD Cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía y servicios|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

