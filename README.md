# 📚 **Sistema de Gestión de Biblioteca - YaviBook**  

¡Bienvenido a **YaviBook**! Un sistema web completo para la gestión de bibliotecas que facilita la administración de **libros**, **usuarios** y **préstamos** de manera eficiente y segura. 🌟

---

## 📝 **Descripción**

**YaviBook** es una solución moderna y escalable diseñada para bibliotecas que necesitan gestionar recursos, usuarios y operaciones de préstamos.  
Este sistema incluye un backend potente, una API RESTful bien estructurada, y una interfaz de usuario interactiva construida con React.

---

## 📂 **Estructura del Proyecto**

### 🛠️ **Backend**
El backend está desarrollado con **Node.js** y **Express**, utilizando **MongoDB** como base de datos. Proporciona un conjunto robusto de endpoints para manejar libros, usuarios y préstamos.

#### **Endpoints API**
##### 📚 **Libros** (`/api/v1/biblioteca`)
- **GET /** - Obtener todos los libros.  
- **GET /:bookId** - Obtener un libro por ID.  
- **DELETE /deleteAll** - Eliminar todos los libros (requiere rol de administrador).  

##### 👥 **Usuarios** (`/api/v1/users`)
- Gestión de usuarios y autenticación.  
- Acceso protegido mediante middleware de autenticación.  

##### 🔄 **Préstamos** (`/api/v1/prestamo`)
- **POST /loans** - Crear un nuevo préstamo.  
- **GET /loans** - Obtener todos los préstamos.  
- **PUT /loans/:id** - Actualizar un préstamo.  
- **DELETE /loans/:id** - Eliminar un préstamo.  

---

### 🌐 **Frontend** (Carpeta `/public`)
El frontend está desarrollado con **React** y compilado para producción con la siguiente estructura:  

  ```plaintext
  public/
  ├── index.html
  ├── manifest.json
  ├── static/
  │   ├── css/
  │   │   └── main.cf86c182.css
  │   └── js/
  │       ├── main.c8ed8e8a.js
  │       └── 787.9e9f4ffd.chunk.js
```
### 🚀 Características
### 🔐 Autenticación y Seguridad
Autenticación de usuarios mediante JWT.
Middleware para la protección de rutas.
Gestión de roles de usuario (admin/regular).
Contraseñas encriptadas con bcryptjs.
### 📘 Gestión de Libros
Registrar, editar y eliminar libros.
Listado completo con opciones de búsqueda.
### 🔄 Sistema de Préstamos
Registrar y gestionar préstamos de libros.
Actualización del estado de los préstamos.
Eliminación de préstamos obsoletos.
### 📊 Panel de Administración
Visualización de estadísticas de préstamos y usuarios.
Gestión centralizada de recursos.
### 🛡️ API RESTful
Endpoints bien estructurados para integrar con cualquier cliente.
### 🎨 Interfaz de Usuario Moderna
Aplicación frontend responsiva desarrollada con React.
Navegación fluida gracias a React Router DOM.
Estilos personalizables con CSS.
### ⚙️ Tecnologías Utilizadas
Backend
Node.js + Express
MongoDB + Mongoose
JWT para autenticación.
bcryptjs para encriptación de contraseñas.
CORS para control de accesos.
Frontend
React
React Router DOM
CSS para estilos.
### 🛠️ Configuración
### 🔑 Variables de Entorno
Asegúrate de configurar un archivo .env con las siguientes claves:

```plaintext
Copiar código
PORT=5000
MONGO_URI=<tu-uri-de-mongodb>
JWT_SECRET=<tu-secreto-jwt>
```
