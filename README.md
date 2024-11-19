# Gestion-gym
# Gestión de Gimnasio 🏋️‍♂️

## Descripción del Proyecto
Este proyecto es un sistema de gestión de gimnasios diseñado para facilitar el manejo de clientes, membresías, planes, facturación y notificaciones. Combina una arquitectura backend en **Java Spring Boot** con un frontend construido en **Ionic** y **Vue.js**. La base de datos está configurada en **MySQL** mediante **XAMPP**.

## Características Principales 🌟
- **Gestión de clientes**: Registro, edición y eliminación de información de clientes.
- **Control de membresías**: Creación, asignación y seguimiento de las membresías activas.
- **Facturación**: Emisión de facturas automatizadas para las membresías adquiridas.
- **Notificaciones**: Sistema para enviar alertas o recordatorios a los clientes.
- **Planes de entrenamiento**: Gestión de los planes disponibles en el gimnasio.

## Tecnologías Utilizadas 🛠️

### Backend
- **Lenguaje**: Java  
- **Framework**: Spring Boot  
- **Entorno de desarrollo**: IntelliJ IDEA  

### Frontend
- **Framework**: Ionic + Vue.js  
- **Editor de código**: Visual Studio Code  

### Base de Datos
- **Sistema gestor**: MySQL  
- **Herramienta**: XAMPP  

## Arquitectura del Sistema 🏗️
El sistema utiliza una arquitectura basada en servicios:
- **Backend (API REST)**: Proporciona endpoints para la gestión de datos, creados con Java Spring Boot.
- **Frontend**: Aplicación web interactiva desarrollada con Ionic y Vue.js.
- **Base de datos**: Almacena las entidades principales y sus relaciones en MySQL.

## Entidades Principales 📊
### Cliente
- **Atributos**: Nombre, Apellido, Edad, Dirección, Email, Teléfono.  

### Membresía
- **Atributos**: Fecha de inicio, Fecha de fin, Tipo, Estado, Cliente asociado.  

### Factura
- **Atributos**: Número, Fecha, Total, Cliente asociado.  

### Plan
- **Atributos**: Nombre, Descripción, Duración, Precio.  

### Notificación
- **Atributos**: Mensaje, Tipo, Fecha, Cliente asociado.  

## Requisitos Previos 🔧

### Backend
- Java JDK 11 o superior  
- Maven  
- IntelliJ IDEA

### Frontend
- Node.js  
- Ionic CLI  
- Visual Studio Code  

### Base de Datos
- XAMPP (para MySQL y phpMyAdmin)  

## Instalación y Configuración 🛠️

### Clonar el repositorio
```
git clone https://github.com/NicolasAlvarez25/Gestion-gym.git
cd Gestion-gym
```
## Configurar el Backend
### Configura el archivo application.properties con los datos de conexión a MySQL:
properties
```
spring.datasource.url=jdbc:mysql://localhost:3306/nombre_base_datos
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update
```

# Ejecuta la aplicación desde IntelliJ IDEA o mediante Maven:
```
mvn spring-boot:run
```

# Configurar el Frontend
## Instala las dependencias:
```
npm install
```

# Ejecuta la aplicación en modo desarrollo:
```
ionic serve
```


# Uso del Sistema 🖥️
## Rutas del Backend (API REST)
### Cliente: /api/clientes GET, POST, PUT, DELETE
## Membresía: /api/membresias 
### GET, POST, PUT, DELETE
## Factura: /api/facturas 
### GET, POST
## Plan: /api/planes 
### GET, POST, PUT
## Notificación: /api/notificaciones
### GET, POST

# Navegación en el Frontend
### Página de inicio: Vista general del sistema.
### Gestión de clientes: Agregar, editar o eliminar clientes.
### Membresías: Consultar y asignar membresías.
### Facturación: Emitir y consultar facturas.
### Notificaciones: Enviar recordatorios o alertas.

# Base de Datos 📂
## Diagrama ER:
### Configuración inicial
### Inicia XAMPP y activa MySQL.
Crea la base de datos con el siguiente comando en phpMyAdmin:
```
sql
CREATE DATABASE nombre_base_datos;
```
Importa el archivo schema.sql para crear las tablas.

# Mejoras Futuras 🚀
### Integración con pasarelas de pago para membresías.
### Notificaciones por correo electrónico o SMS.
### Generación de reportes estadísticos.

# Contribuciones 🤝
### Si deseas contribuir, sigue estos pasos:
### Haz un fork del proyecto.
### Crea una rama nueva (git checkout -b feature/nueva-funcionalidad).
### Realiza tus cambios y súbelos (git commit -m "Descripción de los cambios").
### Envía un pull request.

# Autor ✍️
### Nombre del Autor: [Tu Nombre]
### Contacto: [Tu Email]

# Licencia 📜
### Este proyecto está bajo la licencia MIT. Consulta el archivo LICENSE para más detalles.
