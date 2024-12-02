# 👋 ¡Hola! Soy @CrisDebug

- 👀 Estoy interesado en el desarrollo web y en la creación de aplicaciones de gestión que hagan la vida más sencilla.
- 🌱 Actualmente estoy aprendiendo frameworks modernos de JavaScript como node.js y herramientas para desarrollo backend como Laravel.
- 💞️ Estoy dispuesto a colaborar en proyectos, incluso si no son tan desafiantes, porque mi pasión por la programación va más allá de cualquier funcionalidad.
- 📫 Cómo contactarme: Puedes escribirme a crisdebug@ejemplo.com o conectarte conmigo en [LinkedIn](https://linkedin.com/in/crisdebug).
- 😄 Pronombres: Él/Él (He/Him).
- ⚡ Un dato curioso sobre mí: Me encanta la música tambien soy beatmaker,
- y a veces encuentro inspiración para resolver problemas mientras escucho mi playlist favorita o creo alguna instrumental. 🎵

---

✨ Si también te apasiona programar, no dudes en escribirme. ¡Me encantaría conectar con otros desarrolladores y compartir ideas! 🚀

# Curso App (Aplicación de Cursos)

Este proyecto es una aplicación web de cursos "en proceso de construccion" esta siendo desarrollada con **Laravel**. 
Los usuarios pueden ver, buscar y gestionar cursos. La aplicación utiliza **SQLite** como base de datos porser una base liviana para pruebas , 
de todas manera podria migrar a mysql si es necesario modificacando el archivo de conexiones
para luego ejecutar las migraciones a una nuevabase de datos compatible
, el frontend está optimizado con **Tailwind CSS**.

## Características

- Gestión de cursos (listar, agregar, editar, eliminar).
- Vista de cursos para los usuarios.
- Optimización del frontend con **Tailwind CSS**.
- Uso de **Blade** para las vistas.
- **SQLite** como base de datos.

### ✨ Funcionalidades planeadas:
- Registro de usuarios (estudiantes e instructores).
- Panel de control para la gestión de cursos.
- Integración con pasarelas de pago.
- Sistema de seguimiento del progreso de los estudiantes.
- Diseño responsivo y accesible.

## Requisitos previos

Asegúrate de tener instalados los siguientes programas en tu máquina local:

- **LARAVEL** (versión 7.3 o superior).
- **Composer** (gestor de dependencias para PHP).
- **SQLite** (base de datos).
- **Node.js** y **NPM** (para instalar y compilar dependencias de frontend, como Tailwind CSS).

## Instalación

Sigue estos pasos para poner en marcha la aplicación en tu máquina local:

1. **Clona este repositorio**:
    ```bash
    git clone https://githttps://github.com/CrisDebug/app_cursos.git
    cd app_cursos
    ```

2. **Instala las dependencias de PHP**:
    - Asegúrate de tener **Composer** instalado. Luego, ejecuta:
    ```bash
    composer install
    ```

3. **Configura la base de datos**:
    - Copia el archivo de configuración `.env.example` a `.env`:
    ```bash
    cp .env.example .env
    ```
    - Asegúrate de que la configuración de la base de datos en el archivo `.env` esté configurada para usar **SQLite**:
    ```env
    DB_CONNECTION=sqlite
    DB_DATABASE=database/database.sqlite
    ```

4. **Crea la base de datos**:
    - Si no tienes el archivo `database.sqlite` aún, crea un archivo vacío en la carpeta `database` de tu proyecto:
    ```bash
    touch database/database.sqlite
    ```
    - Luego ejecuta las migraciones:
    ```bash
    php artisan migrate
    ```

5. **Instala las dependencias de frontend** (Tailwind CSS y otras dependencias):
    ```bash
    npm install
    ```

6. **Compila los assets de frontend**:
    - Para compilar y optimizar los archivos CSS:
    ```bash
    npm run dev
    ```

7. **Inicia el servidor local de Laravel**:
    ```bash
    php artisan serve
    ```
    La aplicación estará disponible en [http://localhost:8000](http://localhost:8000).

## Uso

### Agregar Cursos

  Los usuarios pueden agregar cursos a través del mantenedor.

### Frontend

La aplicación está optimizada usando **Tailwind CSS** para una experiencia de usuario moderna y fluida. Las vistas están renderizadas utilizando **Blade**, el motor de plantillas de Laravel.

## Tecnologías Utilizadas

- **Backend**: Laravel 11
- **Base de datos**: SQLite
- **Frontend**: Blade, Tailwind CSS, HTML, CSS
- **Optimización CSS**: Tailwind CSS para diseño responsivo y optimización visual.

## Contribuciones

Si deseas contribuir a este proyecto, por favor sigue los siguientes pasos:

1. Haz un fork del repositorio.
2. Crea una nueva rama (`git checkout -b feature/nueva-caracteristica`).
3. Realiza tus cambios y haz commit (`git commit -am 'Agrega nueva característica'`).
4. Haz un push a tu rama (`git push origin feature/nueva-caracteristica`).
5. Crea un nuevo Pull Request.

### **Explicación de las secciones del README**

- **Nombre y Descripción del Proyecto**: el proyecto trata de una app de una aplicación para la gestion de cursos.
- **Características**: gestión de cursos por mantenedor, frontend optimizado con Tailwind CSS,sqlite para pruebas.
- **Requisitos previos**: las indicaciones esta escritas en la seccion de requisitos previos donde posteriormente se explica el proceso de instalacion
- de lo que sea necesario para que la app funcione correctamente.
- **Instalación**: todas las dependencias necesarias estan definidas en la seccion instalacion
- **Uso**: puedes gragegar cursos en la seccion del mantenedor y probar las funcionalidades que tiene , tambien podrias interactuar con el sistema de autenticacion
- que esta construccion , proximamente tendra roles y permisos asignados, por el momento puedes agregar cursos libremente e interactuar con los distintos items del menu
- la idea es que el usuario posterior a su autenticacion tenga acceso solamente a los cursos disponibles y el usuario escritor pueda realizar cambios en los cursos
- y su tematica, siendo el susuario admin el que administre toda la app.
- **Tecnologías Utilizadas**: tecnologias utilizadas Laravel 11 , SQLite, Blade, Tailwind CSS.
- **Contribuciones**: si deceas aportar a este proyecto puedes ver las intruccione en la seccion de **contribuciones**.


