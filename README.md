# Frontend – Administrador de Productos
Este proyecto es el frontend de una API REST que desarrollé previamente con Express y Sequelize. Está hecho en React y permite crear, visualizar, editar y eliminar productos desde una interfaz web conectada al backend.

## Tecnologías
React – Librería principal para construir la interfaz.
React Router DOM.
Tailwind CSS – Framework de estilos que permite diseñar interfaces y responsivas.
Zod – Librería para validar los datos antes de enviarlos al backend.
Fetcher – Permite realizar acciones como eliminar sin salir de la página, mejorando la experiencia del usuario.
Morgan – Lo usamos para registrar en consola las peticiones HTTP, cuánto tardan, el método usado y la ruta.

## Funcion
La aplicación muestra en su página principal una lista con todos los productos almacenados en la base de datos.
Cuenta con un formulario donde se puede agregar un nuevo producto (nombre y precio).
Al enviar el formulario:
Los datos se validan con Zod, se envían mediante un action al backend usando axios, si todo sale bien, el producto se guarda y se actualiza la lista automáticamente.
Cada producto listado tiene dos botones:
Editar: Lleva a una vista donde se puede modificar el nombre, el precio y el estado de disponibilidad del producto.
Eliminar: Borra el producto directamente desde la vista principal, sin necesidad de recargar.

## Instalacion
Clona este repositorio:
git clone https://github.com/Hugo9591/Rest-Api-Ts-Frontend.git

Instala las dependencias:
npm install
Asegúrate de tener corriendo el backend.

Inicia el servidor de desarrollo:
npm run dev

## Requisitos
Tener Node.js y npm instalados.
Tener corriendo el backend.
Conexión entre frontend y backend permitida (configurar CORS si en el backend).
