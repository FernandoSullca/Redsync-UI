# RedsyncUI

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 18.2.11.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.


RedSync-UI
RedSync-UI es la interfaz de usuario de una aplicación basada en Angular, diseñada para gestionar y consultar issues. El proyecto utiliza Angular con SSR (Server-Side Rendering) y SSG (Static Site Generation) para mejorar el rendimiento y SEO.

Contenido
Características
Requisitos Previos
Instalación
Scripts Disponibles
Estructura del Proyecto
Configuración de SSR y SSG
Contribución
Características
Consultas y creación de Issues: Gestiona y consulta issues desde el frontend.
SSR y SSG: Renderización en el servidor y generación de sitios estáticos para una carga inicial más rápida y mejor SEO.
Gestión de Configuración de Usuario y API Keys: Permite a los usuarios personalizar sus configuraciones y gestionar claves API.
Autenticación: Manejo de autenticación para usuarios registrados.
Requisitos Previos
Node.js v14 o superior
Angular CLI (si no está instalado, consulta la sección Instalación)
Instalación
Clona este repositorio en tu máquina local:

bash
Copiar código
git clone https://github.com/tu-usuario/redsync-ui.git
Navega al directorio del proyecto:

bash
Copiar código
cd redsync-ui
Instala las dependencias:

bash
Copiar código
npm install
Scripts Disponibles
Desarrollar en modo SSR
Para ejecutar la aplicación en modo SSR (Server-Side Rendering) en un entorno de desarrollo:

bash
Copiar código
npm run dev:ssr
Construir la aplicación con SSR
Este comando genera la build de producción para SSR, creando archivos para el cliente y el servidor:

bash
Copiar código
npm run build:ssr
Ejecutar la build de producción con SSR
Para iniciar la aplicación en modo de producción tras la build:

bash
Copiar código
npm run serve:ssr
Ejecutar en modo desarrollo sin SSR
Si deseas ejecutar la aplicación en modo de desarrollo estándar (sin SSR):

bash
Copiar código
ng serve
La aplicación estará disponible en http://localhost:4200.

Estructura del Proyecto
src/app: Contiene los componentes, servicios y módulos de la aplicación.
src/assets: Archivos estáticos como imágenes, íconos y estilos.
src/environments: Configuración para diferentes entornos (desarrollo, producción).
src/main.ts: Punto de entrada para la aplicación en el cliente.
src/main.server.ts: Punto de entrada para la aplicación en el servidor (SSR).
server.ts: Configuración del servidor para manejar las solicitudes y renderizar las vistas en el servidor.
Configuración de SSR y SSG
El proyecto está configurado para soportar SSR y SSG, lo cual mejora el rendimiento inicial y la accesibilidad del contenido para los motores de búsqueda.

Consideraciones para SSR
Evita usar directamente objetos del navegador como window o document en tus componentes. Utiliza PLATFORM_ID de Angular para verificar si el código se ejecuta en el navegador o en el servidor.
Puedes verificar el entorno de ejecución con:
typescript
Copiar código
import { isPlatformBrowser } from '@angular/common';
Contribución
Para contribuir a este proyecto:

Haz un fork del repositorio.
Crea una rama con una nueva característica (git checkout -b feature/nueva-caracteristica).
Realiza tus cambios y haz commit (git commit -m 'Agrega nueva característica').
Sube tus cambios (git push origin feature/nueva-caracteristica).
Abre un Pull Request en este repositorio.
Licencia
Este proyecto está bajo la licencia MIT.