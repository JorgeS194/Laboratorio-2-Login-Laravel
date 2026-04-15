# 🧪 Laboratorio Laravel - Implementación de Login (MVC)

## 📌 Introducción

Este laboratorio tiene como objetivo realizar un primer acercamiento al framework Laravel, comprendiendo su estructura basada en el patrón **Modelo-Vista-Controlador (MVC)**.

Laravel organiza el desarrollo en tres componentes principales:
* **Modelos (Models):** Representan la estructura de la base de datos y la lógica del negocio.
* **Vistas (Views):** Encargadas de la interfaz gráfica que ve el usuario.
* **Controladores (Controllers):** Gestionan la comunicación entre modelos y vistas.

Además, se trabajó con rutas (`routes/web.php`) que permiten definir el acceso a las distintas funcionalidades del sistema.

El objetivo principal fue implementar un sistema de **registro y login de usuarios**, utilizando las herramientas que Laravel ofrece por defecto.


## ⚙️ Requisitos Previos

### 🖥️ Entorno de Desarrollo

* Sistema Operativo: Windows
* Servidor local: WAMP

### 🧰 Tecnologías utilizadas

* PHP >= 8.0
* Composer
* Laravel Installer
* Node.js
* NPM
* MySQL
* Apache
* Visual Studio Code



## 🚀 Instalación y Configuración

### 📥 Instalación del proyecto

```
composer global require laravel/installer
laravel new example-app
```

### 📦 Instalación de dependencias

```
composer install
```

### 🔐 Configuración de entorno

Editar el archivo `.env`:

```
DB_CONNECTION=mysql
DB_DATABASE=nombre_bd
DB_USERNAME=root
DB_PASSWORD=
```



## 🗄️ Base de Datos

Se utilizó **MySQL** como gestor de base de datos.

### 📌 Migraciones

```
php artisan migrate
```

Este comando permite:

* Crear las tablas necesarias
* Gestionar cambios en la base de datos
* Mantener control de versiones de la estructura



## 🔑 Generación de clave de aplicación

```bash
php artisan key:generate
```

Esto genera la clave `APP_KEY`, necesaria para la seguridad del sistema.



## 🧹 Limpieza de caché de configuración

```
php artisan config:cache
```

Permite que Laravel reconozca correctamente los cambios en `.env`.



## 🔐 Implementación de Autenticación (Login)

Se utilizó **Laravel UI** para generar el sistema de autenticación.

### 📦 Instalación del paquete

```
composer require laravel/ui
```

### 🎨 Generación de vistas con Bootstrap

```
php artisan ui bootstrap
php artisan ui bootstrap --auth
```

Esto crea:

* Login
* Registro
* Recuperación de contraseña



## 🎨 Instalación de dependencias Frontend

```
npm install
npm run dev
```

También se utilizó:

```
composer run dev
```

Para compilar los recursos del frontend utilizando Vite.



## ▶️ Ejecución del Proyecto

```
php artisan serve
```

Luego acceder a:

```
http://127.0.0.1:8000/
```



## 🖼️ Resultado del Laboratorio

![Resultado1]("C:\Users\Sarmi\Documents\ESTE SEMESTRE\DS-VII\4. Actividades o Asignaciones\2. Laboratorios o talleres\Laboratorio 2\registro-laravel.jpg")




## ⚠️ Dificultades y Soluciones

### ❌ Error en migraciones

* Problema: Error al ejecutar `php artisan migrate`
* Solución: Verificar configuración en `.env` y conexión a MySQL

### ❌ Error de clave de aplicación

* Problema: `The application encryption key has not been specified`
* Solución:

```
php artisan key:generate
```

### ❌ Problemas con dependencias

* Problema: Errores en frontend
* Solución:

```bash
npm install
npm run dev
```



## 📚 Referencias

* Documentación oficial de Laravel
  [https://laravel.com/docs](https://laravel.com/docs)

* Guía de Laboratorio de Login en Laravel (UTP) 

* Documentación de Composer
  [https://getcomposer.org](https://getcomposer.org)



## 📅 Fecha de Ejecución

**14 de abril de 2026**



## 👨‍💻 Información del Estudiante

Este laboratorio ha sido desarrollado por el estudiante de la Universidad Tecnológica de Panamá:

* **Nombre:** Jorge Sarmiento
* **Cédula:** 3-757-1758
* **Correo:** [jorge.sarmiento@utp.ac.pa](mailto:jorge.sarmiento@utp.ac.pa)
* **Curso:** Desarrollo de Software VII
* **Instructor:** Irina Fong



# 🚀 Notas Finales

Este laboratorio permitió comprender la estructura de Laravel, el uso del patrón MVC y la implementación de un sistema de autenticación funcional, sentando bases importantes para el desarrollo web moderno.
