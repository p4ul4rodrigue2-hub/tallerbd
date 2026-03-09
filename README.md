AutoMarket Pro
AutoMarket Pro es una aplicación robusta diseñada para gestionar el flujo completo de una compraventa de vehículos. El proyecto abarca desde el modelado relacional de datos hasta la implementación de una API RESTful, permitiendo el control de inventario, usuarios (compradores/vendedores) y transacciones.

🚀 Características Principales
Arquitectura Escalable: Desarrollado con Node.js y Express.

Base de Datos Relacional: Diseño normalizado en MySQL (1FN, 2FN, 3FN).

Gestión de Archivos: Implementación de Multer para la subida de imágenes de vehículos.

Carga Masiva: Soporte para importación de datos mediante archivos CSV.

CRUD Completo: Gestión de Vehículos, Usuarios y Contratos de Compraventa.

🛠️ Stack Tecnológico
Backend: Node.js, Express.js

Base de Datos: MySQL

Herramientas: Multer (Manejo de archivos), CSV-Parser.

📋 Requisitos Previos
Antes de empezar, asegúrate de tener instalado:

Node.js (v14 o superior)

MySQL Server

🔧 Instalación y Configuración
Clona el repositorio:

Bash
git clone https://github.com/tu-usuario/automarket-pro.git
cd automarket-pro
Instala las dependencias:

Bash
npm install
Configura la Base de Datos:

Crea una base de datos en MySQL llamada automarket_db.

Ejecuta el script de creación de tablas ubicado en /database/script.sql.

Variables de Entorno:
Crea un archivo .env en la raíz y configura tus credenciales:

Fragmento de código
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=tu_password
DB_NAME=automarket_db
PORT=3000
Inicia el servidor:

Bash
npm run dev
📐 Modelo de Datos (MER)
El sistema sigue un modelo relacional estrictamente normalizado para garantizar la integridad de la información, separando las entidades de:

Vehículos: (Placa, Modelo, Marca, Precio, Estado).

Usuarios: (Vendedores y Compradores con roles definidos).

Transacciones: (Registro histórico de ventas y contratos).
