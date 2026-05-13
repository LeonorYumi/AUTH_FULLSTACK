# AUTH_FULLSTACK - REGISTRO

Este proyecto es un sistema funcional de registro, verificación y recuperacion de contraseña mediandte tokens de seguridad.

## Funcionalidades del Sistema
El sistema permite ejecutar un flujo completo de gestión de identidad basado en tokens:

1.  **Registro de Usuario**: Creación de nuevas cuentas desde la interfaz web.
2.  **Verificación de Cuenta**: El sistema genera un `verificationToken` necesario para activar la cuenta a través de la ruta `/verify/TOKEN`.
3.  **Solicitud de Recuperación**: Permite solicitar el restablecimiento de acceso para cuentas existentes.
4.  **Cambio de Contraseña**: Uso de un `resetToken` para establecer una nueva clave mediante la ruta `/reset-password/TOKEN`.

## Tecnologías Utilizadas

### Backend
*   **Node.js & Express**: Framework para la creación de la API y manejo de lógica de tokens.
*   **MongoDB Atlas**: Base de datos NoSQL para el almacenamiento de usuarios y estados de tokens.
*   **Mongoose**: Modelado de datos y comunicación con la base de datos.
*   **Nodemailer**: Integración para el envío de tokens a través de correo electrónico.

### Frontend
*   **React + Vite**: Framework principal para una interfaz rápida y moderna.
*   **Tailwind CSS**: Para el diseño y estilizado de los formularios.
*   **Axios**: Cliente HTTP para la comunicación con el backend.

## Configuración de Entorno

Para que el proyecto funcione correctamente, debes configurar los siguientes archivos `.env`:

### Backend (`/backend/.env`)
```env
PORT=3000
MONGO_URI=tu_conexion_mongodb_atlas
JWT_SECRET=tu_clave_secreta
EMAIL_USER=tu_correo@gmail.com
EMAIL_PASS=tu_app_password_de_google

### Instalación y ejecución
1. **Clonar el repositorio**
git clone [https://github.com/LeonorYumi/AUTH_FULLSTACK.git](https://github.com/LeonorYumi/AUTH_FULLSTACK.git)
cd AUTH_FULLSTACK

2. **Ejecutar el backend**
cd backend
npm install
npm run dev

3. **Ejecutar el Frontend**
cd ../frontend
npm install
npm run dev


