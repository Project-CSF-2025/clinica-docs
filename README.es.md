# Sistema de Reportes de Incidentes Clínicos – Descripción General del Proyecto

Esta es una aplicación web full-stack diseñada para permitir que el personal hospitalario o clínico envíe reportes de incidentes de forma anónima. El sistema mejora la comunicación y la seguridad al permitir interacciones seguras y rastreables entre el personal y los administradores.

Este proyecto está dividido en dos repositorios separados:

- 🔗 [Repositorio del Frontend](https://github.com/Project-CSF-2025/clinica-front-public)  
- 🔗 [Repositorio del Backend](https://github.com/Project-CSF-2025/clinica-back-public)

---

## Resumen del Proyecto

La aplicación permite al personal clínico reportar incidentes mediante un formulario anónimo, y a los administradores gestionar esos reportes en un panel privado. Cada reporte se rastrea con un código único, lo que permite comunicación y seguimiento sin revelar la identidad del usuario.

---

## Tecnologías Utilizadas

### Frontend:
- React (con Vite)
- JavaScript (ES6+)
- Bootstrap y MUI
- Configuración de entorno mediante `.env`

### Backend:
- Node.js con Express
- SQL Server
- Autenticación con JWT
- Multer para la gestión de archivos
- Nodemailer para envío de correos electrónicos

---

## 🔧 Cómo Funciona

- **Usuarios** pueden:
  - Completar y enviar un formulario de reporte anónimo
  - Adjuntar archivos opcionales (imágenes o PDFs)
  - Proporcionar un correo electrónico opcional para recibir notificaciones

- **Administradores** pueden:
  - Iniciar sesión de forma segura con autenticación JWT
  - Ver reportes, actualizar estados y agregar notas internas
  - Intercambiar mensajes con usuarios anónimos
  - Descargar archivos y datos

---

## Comunicación entre Frontend y Backend

- El frontend usa una variable de entorno `.env` (`VITE_API_URL`) para definir la URL base de la API.
- El backend expone rutas para reportes, mensajes, login, seguimiento de estados y gestión de archivos.
- Se habilita CORS para permitir la comunicación entre frontend y backend.

---

## Desglose de Repositorios

### 🔸 Repositorio del Backend

**URL:** [clinica-back-public](https://github.com/Project-CSF-2025/clinica-back-public)

Incluye:

- Sistema de login para administradores con JWT
- Lógica de carga de archivos con Multer
- Notificaciones por correo electrónico con Nodemailer
- Esquema de base de datos en SQL Server
- Gestión de reportes anónimos
- Documentación completa del archivo `.env` y configuración

### 🔸 Repositorio del Frontend

**URL:** [clinica-front-public](https://github.com/Project-CSF-2025/clinica-front-public)

Incluye:

- Formulario para reportes anónimos
- Panel administrativo en la ruta `/admin`
- Interfaz de mensajería para seguimientos
- Visualización de reportes y filtros de estado
- Menús desplegables configurables mediante archivos JSON (departamentos, profesiones, etc.)

---

## Autoras

- **Pragati Juyal** – Desarrollo del backend y coordinación full-stack  
- **Kanako Inamine** – Desarrollo del frontend y diseño UI/UX

---

## Licencia

Este proyecto está licenciado bajo la [Licencia MIT](./LICENSE).  
Se proporciona "tal cual" y las autoras no se hacen responsables de posibles daños.  
Se permite su uso en producción siempre que se otorgue el crédito correspondiente.
