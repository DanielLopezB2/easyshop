# API CRUD para Ecommerce

Este repositorio contiene el código fuente para una API RESTful de ecommerce que gestiona productos, permitiendo realizar operaciones CRUD (crear, leer, actualizar y eliminar). La API está construida usando Spring Boot y utiliza Hibernate para la persistencia de datos con MySQL.

## Tabla de Contenidos
- [Requisitos Previos](#requisitos-previos)
- [Configuración del Proyecto](#configuración-del-proyecto)
- [Instrucciones de Instalación](#instrucciones-de-instalación)
- [Ejecución del Proyecto](#ejecución-del-proyecto)
- [Uso de la API](#uso-de-la-api)

## Requisitos Previos

Antes de comenzar, asegúrate de tener instalados los siguientes requisitos:

1. **Java 17 o superior**: Asegúrate de tener una versión compatible de Java instalada.
2. **Maven**: Utilizado para la gestión de dependencias y la construcción del proyecto.
3. **MySQL**: Base de datos relacional utilizada para la persistencia de los datos.
4. **Postman o cURL**: Herramientas recomendadas para probar la API.

## Configuración del Proyecto

### 1. Clonar el Repositorio

```bash
git clone https://github.com/usuario/ecommerce-crud-api.git
cd ecommerce-crud-api
```

### 2. Configurar la Base de Datos

1. **Crea una base de datos en MySQL llamada `db_easyshop`:**

```sql
CREATE DATABASE db_easyshop;
```

2. Configura las credenciales de tu base de datos MySQL en el archivo
```
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```
### 3. Uso de la API

**Crear producto**

#### POST /products

```
{
  "name": "Producto Ejemplo",
  "description": "Descripción del producto",
  "price": 19.99,
  "category": "Electrónica",
  "stock": 100
}
```
#### GET /products

#### GET /products/{id}

#### PUT /products/{id}
```
{
  "name": "Producto Ejemplo",
  "description": "Descripción del producto",
  "price": 19.99,
  "category": "Electrónica",
  "stock": 100
}

```

#### DELETE /products/{id}

