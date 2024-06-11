# Sistema de Pedidos para Restaurante

Este proyecto implementa un sistema de pedidos para un restaurante utilizando Node.js, Express y MySQL.

## Características

- Permite a los clientes realizar pedidos mediante un formulario web.
- Calcula automáticamente el subtotal y total del pedido, incluyendo una propina del 10%.
- Almacena los pedidos en una base de datos MySQL.

## Tecnologías Utilizadas

- **Node.js** - Entorno de ejecución para JavaScript.
- **Express** - Framework web para Node.js.
- **MySQL** - Sistema de gestión de base de datos relacional.
- **HTML/CSS** - Frontend básico para el formulario de pedidos.

## Instalación

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/tu_usuario/tu_repositorio.git
   cd tu_repositorio

2. **instala las dependencias**
   ```bash
   npm install express mysql body-parser

3. Estructura
   ```bash
   /restaurant-order
   |-- /db
   |   |-- connection.js
   |-- /models
   |   |-- order.js
   |-- /public
   |   |-- styles.css
   |   |-- scripts.js
   |   |-- index.html
   |-- /routes
   |   |-- orders.js
   |-- app.js
   |-- package.json
   |-- README.md

4. Configuración de la Base de Datos con XAMPP:

Asegúrate de tener XAMPP instalado y en ejecución.

Abre el panel de control de XAMPP y enciende Apache y MySQL.

Abre phpMyAdmin desde el panel de control de XAMPP.

Crea una nueva base de datos llamada restaurant.

```bash
CREATE DATABASE restaurant;
USE restaurant;
CREATE TABLE orders (
    id INT AUTO_INCREMENT PRIMARY KEY,
    table_number INT NOT NULL,
    items TEXT NOT NULL,
    subtotal DECIMAL(10, 2) NOT NULL,
    total DECIMAL(10, 2) NOT NULL
);




