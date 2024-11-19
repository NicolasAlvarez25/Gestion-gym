# Gestion-gym
# Gestión de Gimnasio 🏋️‍♂️

## Descripción del Proyecto
Este proyecto es un sistema de gestión de gimnasios diseñado para facilitar el manejo de clientes, membresías, planes, facturación y notificaciones. Combina una arquitectura backend en **Java Spring Boot** con un frontend construido en **Ionic** y **Vue.js**. La base de datos está configurada en **MySQL** mediante **XAMPP**.

## Alcance del Proyecto 🏋️‍♂️
El sistema de Gestión de Gimnasios tiene como objetivo optimizar los procesos administrativos y operativos de un gimnasio mediante la implementación de un software robusto y fácil de usar. Este proyecto se enfoca en la gestión eficiente de clientes, membresías, facturación, planes de entrenamiento y notificaciones.

## Objetivos Generales
Desarrollar un sistema completo que permita la administración de un gimnasio, abarcando desde la gestión de clientes hasta el seguimiento de pagos y servicios.

## Objetivos Específicos

- *Gestión de Clientes*:
Registrar, actualizar y eliminar información de clientes.
Consultar el historial de membresías y pagos asociados a cada cliente.

- *Administración de Membresías*:
Crear y asignar membresías personalizadas a clientes según sus necesidades.
Administrar fechas de inicio, vencimiento y renovación de membresías.

- *Facturación*:
Generar facturas detalladas para cada cliente.
Consultar el estado de pagos (pagado o pendiente).

- *Planes de Entrenamiento*:
Crear y gestionar planes de entrenamiento personalizados para los clientes.
Asociar planes de entrenamiento con membresías o servicios contratados.

- *Notificaciones*:
Enviar recordatorios automáticos a los clientes sobre fechas de pago, vencimientos de membresías y promociones especiales.
Funcionalidades Incluidas
Frontend (Interfaz de Usuario):

Diseño responsive que permite su uso en dispositivos móviles y computadoras.
Interfaz intuitiva desarrollada con Ionic + Vue.js para facilitar la experiencia del usuario.

- *Backend*:
API REST implementada en Java Spring Boot para gestionar las operaciones del sistema.
Integración con una base de datos MySQL para almacenamiento de información.

- *Base de Datos*:
Tablas diseñadas para almacenar información de clientes, membresías, facturación, planes y notificaciones.
Scripts predefinidos para la creación y población de datos iniciales.

- *Automatización*:
Generación de notificaciones automáticas para pagos y vencimientos.
Actualización en tiempo real de datos mediante la sincronización entre backend y frontend.

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
spring.datasource.url=jdbc:mysql://localhost:3307/FitManage?useSSL=false&serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
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


## Uso del Sistema 🖥️
Rutas del Backend (API REST)
- *Cliente*: /api/clientes
- GET, POST, PUT, DELETE
- *Membresía*: /api/membresias
-  GET, POST, PUT, DELETE
- *Factura* : /api/facturas
- GET, POST
- *Plan*: /api/planes
- GET, POST, PUT
- *Notificación*: /api/notificaciones
-  GET, POST

## Navegación en el Frontend
 Página de inicio: Vista general del sistema.
 Gestión de clientes: Agregar, editar o eliminar clientes.
 Membresías: Consultar y asignar membresías.
 Facturación: Emitir y consultar facturas.
 Notificaciones: Enviar recordatorios o alertas.

## Base de Datos 📂
 Diagrama ER:
 Configuración inicial
 Inicia XAMPP y activa MySQL.
Crea la base de datos con el siguiente comando en phpMyAdmin:
```
sql
CREATE DATABASE FitManage;
```
Importa el archivo schema.sql para crear las tablas.

## Mejoras Futuras 🚀
 Integración con pasarelas de pago para membresías.
 Notificaciones por correo electrónico o SMS.
 Generación de reportes estadísticos.
