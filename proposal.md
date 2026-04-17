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

## Tema: SportBook
### Descripción
*Aplicación que permite a los usuarios reservar canchas deportivas dentro de un complejo , gestionando horarios disponibles, reservas y administración del sistema.*

### Modelo
<img width="4672" height="6135" alt="User and Reservation-2026-04-17-042924" src="https://github.com/user-attachments/assets/4aeed8fe-3fce-4304-afba-75565c65f084" />

Link con la imagen del modelo de dominio: [https://mermaid.ai/app/projects/e33a41a0-43dd-4124-b776-9b6882c04f7d/diagrams/1ec81a37-bb9c-4a99-b88e-4cb14f082692/share/invite/eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJkb2N1bWVudElEIjoiMWVjODFhMzctYmI5Yy00YTk5LWI4OGUtNGNiMTRmMDgyNjkyIiwiYWNjZXNzIjoiQ29tbWVudCIsImlhdCI6MTc3NjQwMTM1NH0.I6Px--gVPHryBvjZcAeUfpaIoc6KpST5bADxA_eow](https://mermaid.ai/app/projects/e33a41a0-43dd-4124-b776-9b6882c04f7d/diagrams/1ec81a37-bb9c-4a99-b88e4cb14f082692/share/invite/eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJkb2N1bWVudElEIjoiMWVjODFhMzctYmI5Yy00YTk5LWI4OGUtNGNiMTRmMDgyNjkyIiwiYWNjZXNzIjoiQ29tbWVudCIsImlhdCI6MTc3NjQwMTQ3OX0.wAi_50E74Y_OZSxy6gFUXDGzYGfR4IT-6-E7IgpKOKw)

## Alcance Funcional 

### Alcance Mínimo
 

| Req                     | Detalle                                                                                                                                                                                                                                                                   |
| :---------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| CRUD simple             | 1. CRUD TipoCancha<br>2. CRUD TipoEvento<br>3. CRUD Equipamiento                                                                                                                                                                                                          |
| CRUD dependiente        | 1. CRUD Cancha {depende de} CRUD TipoCancha<br>2. CRUD Reserva {depende de} CRUD Usuario y CRUD Cancha                                                                                                                                                                    |
| Listado<br>+<br>detalle | 1. Listado de canchas filtrado por tipo de cancha, muestra nombre y precio => detalle CRUD Cancha<br>2. Listado de reservas filtrado por fecha o cancha, muestra fecha, horario, estado y usuario => detalle muestra datos completos de la reserva, evento y equipamiento |
| CUU/Epic | 1. Reservar una cancha<br>2. Gestionar reservas (cancelar/modificar) |                                                                                                                               |



Adicionales para Aprobación
| Req      | Detalle                                                                                                                                                    |
| :------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CRUD     | 1. CRUD Usuario<br>2. CRUD TipoCancha<br>3. CRUD Cancha<br>4. CRUD Reserva<br>5. CRUD Evento<br>6. CRUD TipoEvento<br>7. CRUD Equipamiento<br>8. CRUD Pago |
| CUU/Epic | 1. Reservar una cancha<br>2. Cancelar/modificar reserva<br>3. Registrar pago de una reserva |



### Alcance Adicional Voluntario

| Req      | Detalle                                                                                                                     |
| :------- | :-------------------------------------------------------------------------------------------------------------------------- |
| Listados | 1. Listado de reservas por usuario mostrando historial<br>2. Listado de disponibilidad por cancha y fecha (tipo calendario) |
| CUU/Epic | 1. Cancelación automática con penalización<br>2. Agregar equipamiento a una reserva existente                               |
| Otros    | 1. Notificación de confirmación de reserva (email o simulación)<br>2. Validación de no superposición de reservas            |


