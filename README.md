Propuesta TP DSW - ISI COM 302 - 2025
Grupo (FitCenter)
Integrantes
legajo - Apellido(s), Nombre(s)
52612-Egidi, Kevin
52267-Bercini, Genaro
52806-Piccoli, Nicolas
53038-Cravero, Tomas
52107-Rojtberg, Ramiro
Repositorios
FrontEnd
BackEnd
Tema
Descripción
FitCenter es un sistema web diseñado para gestionar de forma integral las actividades de un gimnasio, facilitando la interacción entre tres roles principales: clientes, profesores y administradores. La plataforma ofrece funcionalidades como la reserva de horarios de entrenamiento, la creación y asignación de rutinas personalizadas, la gestión de membresías y la venta de productos deportivos a través de una tienda online, que incluye una pasarela de pagos.

Modelo
DER

Alcance Funcional
Alcance Mínimo
Regularidad:

Req	Detalle
CRUD simple	1. CRUD Usuarios
2. CRUD Membresias
3. CRUD Productos
4. CRUD Ejercicios
5. CRUD Categorias
6. CRUD Sucursales
7. CRUD Turnos
CRUD dependiente	1. CRUD Rutinas {depende de} CRUD Profesores
2. CRUD OrdenesCompra {depende de} CRUD Productos y CRUD Cliente
3. CRUD Cupos {depende de} CRUD Sucursales y CRUD Turnos
Listado
+
detalle	1. Listado de Productos filtrado por categorias, muestra nombre y precio => detalle CRUD Productos
2. Listado de Turnos busqueda por fecha unica y filtrado por fechas disponibles, muestra fecha de Turnos, fecha inicio de Turnos, cantidad de Cupos disponibles => detalle muestra datos completos del Turno y del Cliente
CUU/Epic	1. Cargar Productos
2. Comprar un Producto
Adicionales para Aprobación

Req	Detalle
CRUD	1. CRUD Usuarios
2. CRUD Membresias
3. CRUD Productos
4. CRUD Ejercicios
5. CRUD Categorias
6. CRUD Sucursales
7. CRUD Turnos
8. CRUD Rutinas {depende de} CRUD Profesores
9. CRUD OrdenesCompra {depende de} CRUD Productos y CRUD Cliente
10. CRUD Cupos {depende de} CRUD Sucursales y CRUD Turnos
CUU/Epic	1. Crear Rutinas
2. Reservar un Turno
3. Cargar Ejercicios
4. Cargar Categoria
5. Subscribirse a una Clase
Alcance Adicional Voluntario
Req	Detalle
Listados	1. Clases filtradas por Sucursales
2. Ordenes de compra ordenados por fecha y filtrado por estado
CUU/Epic	1. Cancelar Turno
2. Registrar un Usuario
Otros	1. Envío de confirmacion del turno por email
