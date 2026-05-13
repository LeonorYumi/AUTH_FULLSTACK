# AUTH_FULLSTACK - REGISTRO

Este proyecto es un sistema funcional de registro, verificación y recuperacion de contraseña mediante tokens de seguridad.

## Funcionalidades

El sistema permite ejecutar un flujo completo de gestión de identidad basado en tokens:

1.  **Registro de Usuario**: Creación de nuevas cuentas desde la interfaz web.
2.  **Verificación de Cuenta**: El sistema genera un `verificationToken` necesario para activar la cuenta a través de la ruta `/verify/TOKEN`.
3.  **Solicitud de Recuperación**: Permite solicitar el restablecimiento de acceso para cuentas existentes.
4.  **Cambio de Contraseña**: Uso de un `resetToken` para establecer una nueva clave mediante la ruta `/reset-password/TOKEN`.

## Tecnologías utilizadas

### Backend
*   **Node.js & Express**: Framework para la creación de la API y manejo de lógica de tokens.
*   **MongoDB Atlas**: Base de datos NoSQL para el almacenamiento de usuarios y estados de tokens.
*   **Mongoose**: Modelado de datos y comunicación con la base de datos.
*   **Nodemailer**: Integración para el envío de tokens a través de correo electrónico.

### Frontend
*   **React + Vite**: Framework principal para una interfaz rápida y moderna.
*   **Tailwind CSS**: Para el diseño y estilizado de los formularios.
*   **Axios**: Cliente HTTP para la comunicación con el backend.


## Variables de entorno

- Este proyecto utiliza variables de entorno para la configuración.
- El archivo `.env` no está incluido en el repositorio por seguridad.
  Ejemplo de variables necesarias:
  ```env
PORT=3000
MONGO_URI=tu_conexion_mongodb_atlas
JWT_SECRET=tu_clave_secreta
EMAIL_USER=tu_correo@gmail.com
EMAIL_PASS=tu_app_password_de_google

### Instalación y ejecución del proyecto
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


## Capturas del sistema

1. Registro de cuenta 
   
<img width="1257" height="635" alt="image" src="https://github.com/user-attachments/assets/6f050348-abc5-439f-8441-ebe104ce9126" />

2. Recuperar contraseña

  <img width="1228" height="648" alt="image" src="https://github.com/user-attachments/assets/73b5e87b-6a4b-4253-a6c9-5fe3c92a0f72" />


3. Cambiar contraseña
   
  <img width="1493" height="652" alt="image" src="https://github.com/user-attachments/assets/66d0e533-7184-46b0-8c5f-a8be1e7b6a5c" />


4. Contraseña actualizada correctamente

   <img width="1403" height="541" alt="image" src="https://github.com/user-attachments/assets/6b205cec-ffd4-4e11-af62-fe4886f64b31" />
   

5. Usuarios registrados en Base de Datos MongoDB

<img width="1189" height="715" alt="image" src="https://github.com/user-attachments/assets/96c50738-5ddb-4edf-89f9-77488a015aef" />



## Autor
- Nombres: Leonor Yumi
- Institución: Escuela Politécnica Nacional
