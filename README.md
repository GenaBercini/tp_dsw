# Propuesta TP DSW - ISI COM 302 - 2025

## Grupo (FitCenter)
### Integrantes
* legajo - Apellido(s), Nombre(s)			     
52612-Egidi, Kevin<br>52267-Bercini,	Genaro<br>52806-Piccoli, Nicolas<br>53038-Cravero, Tomas<br>52107-Rojtberg, Ramiro

### Repositorios
* [FrontEnd](https://github.com/ReyKevin1/fitcenter-front)
* [BackEnd](https://github.com/ReyKevin1/fitcenter-back)

## Tema
### Descripción
FitCenter es un sistema web diseñado para gestionar de forma integral las actividades de un gimnasio, facilitando la interacción entre tres roles principales: clientes, profesores y administradores. La plataforma ofrece funcionalidades como la reserva de horarios de entrenamiento, la creación y asignación de rutinas personalizadas, la gestión de membresías y la venta de productos deportivos a través de una tienda online, que incluye una pasarela de pagos.

### Modelo
![DER](DER.png)

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuarios<br>2. CRUD Membresias<br>3. CRUD Productos<br>4. CRUD Ejercicios<br>5. CRUD Categorias<br>6. CRUD Sucursales<br>7. CRUD Turnos<br>|
|CRUD dependiente|1. CRUD Rutinas {depende de} CRUD Profesores<br>2. CRUD OrdenesCompra {depende de} CRUD Productos y CRUD Cliente<br>3. CRUD Cupos {depende de} CRUD Sucursales y CRUD Turnos<br>|
|Listado<br>+<br>detalle| 1. Listado de Productos filtrado por categorias, muestra nombre y precio => detalle CRUD Productos<br> 2. Listado de Turnos busqueda por fecha unica y filtrado por fechas disponibles, muestra fecha de Turnos, fecha inicio de Turnos, cantidad de Cupos disponibles  => detalle muestra datos completos del Turno y del Cliente|
|CUU/Epic|1. Cargar Productos<br>2. Comprar un Producto<br>

Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Usuarios<br>2. CRUD Membresias<br>3. CRUD Productos<br>4. CRUD Ejercicios<br>5. CRUD Categorias<br>6. CRUD Sucursales<br>7. CRUD Turnos<br>8. CRUD Rutinas {depende de} CRUD Profesores<br>9. CRUD OrdenesCompra {depende de} CRUD Productos y CRUD Cliente<br>10. CRUD Cupos {depende de} CRUD Sucursales y CRUD Turnos<br>|
|CUU/Epic|1. Crear Rutinas<br>2. Reservar un Turno<br>3. Cargar Ejercicios<br>4. Cargar Categoria<br>5. Subscribirse a una Clase<br>|

### Alcance Adicional Voluntario

|Req|Detalle|
|:-|:-|
|Listados |1. Clases filtradas por Sucursales <br>2. Ordenes de compra ordenados por fecha y filtrado por estado|
|CUU/Epic|1. Cancelar Turno<br>2. Registrar un Usuario|
|Otros|1. Envío de confirmacion del turno por email|

