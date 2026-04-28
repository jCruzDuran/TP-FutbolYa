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
<img width="5207" height="5830" alt="TP SportBook-2026-04-28-202225" src="https://github.com/user-attachments/assets/489390f0-72b4-4335-af4f-ba4b0ddc7f1b" />

Link con la imagen del modelo de dominio:https://mermaid.ai/app/projects/e33a41a0-43dd-4124-b776-9b6882c04f7d/diagrams/1ec81a37-bb9c-4a99-b88e-4cb14f082692/version/v0.1/edit

## Alcance Funcional 

### Alcance Mínimo
 

| Req                     | Detalle                                                                                                                                                                                                                                                                   |
| :---------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| CRUD simple             | 1. CRUD TipoCancha<br>2. CRUD TipoEvento<br>3. CRUD Equipamiento                                                                                                                                                                                                          |
| CRUD dependiente        | 1. CRUD Cancha {depende de} CRUD TipoCancha<br>2. CRUD Evento {depende de} CRUD TipoEvento                                                                                                                                                                    |
| Listado<br>+<br>detalle | 1. Listado de canchas filtrado por tipo de cancha, muestra nombre y precio => detalle CRUD Cancha<br>2. Listado de reservas filtrado por fecha o cancha, muestra fecha, horario, estado y usuario => detalle muestra datos completos de la reserva, evento y equipamiento |
| CUU/Epic | 1. Reservar una cancha<br>2. Gestionar reservas (cancelar/modificar) |                                                                                                                               |



Adicionales para Aprobación
| Req      | Detalle                                                                                                                                                    |
| :------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CRUD     | 1. CRUD Usuario<br>2. CRUD TipoCancha<br>3. CRUD Cancha<br>4. CRUD Evento<br>5. CRUD TipoEvento<br>6. CRUD Equipamiento<br>7. CRUD Pago |
| CUU/Epic | 1. Reservar una cancha<br>2. Cancelar/modificar reserva<br>3. Registrar pago de una reserva |



### Alcance Adicional Voluntario

| Req      | Detalle                                                                                                                     |
| :------- | :-------------------------------------------------------------------------------------------------------------------------- |
| Listados | 1. Listado de reservas por usuario mostrando historial<br>2. Listado de disponibilidad por cancha y fecha (tipo calendario) |
| CUU/Epic | 1. Cancelación automática con penalización<br>2. Agregar equipamiento a una reserva existente                               |
| Otros    | 1. Notificación de confirmación de reserva (email o simulación)<br>2. Validación de no superposición de reservas            |


