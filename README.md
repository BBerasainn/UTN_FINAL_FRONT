TP Final – Frontend

Este es el frontend del Trabajo Final de la curso Fullstack.
La aplicación permite registro, verificación por email, inicio de sesión y un chat básico.

1. Tecnologías utilizadas

React

Vite

Tailwind CSS

React Router DOM

Axios

Context API

localStorage

2. Estructura del proyecto
src/
 ├── api/
 │    └── axios.js
 ├── components/
 │    ├── ChatItem.jsx
 │    ├── ChatList.jsx
 │    ├── ChatSidebar.jsx
 │    ├── ChatView.jsx
 │    ├── EditContactModal.jsx
 │    ├── MessageBubble.jsx
 │    └── MessageInput.jsx
 ├── contexts/
 │    └── AuthContext.jsx
 ├── pages/
 │    ├── Login.jsx
 │    ├── Register.jsx
 │    ├── VerifyAccount.jsx
 │    └── ChatPage.jsx
 ├── routes/
 │    └── AppRouter.jsx
 ├── App.jsx
 ├── main.jsx
 └── index.html

3. Variables de entorno

El frontend utiliza una sola variable de entorno:

VITE_API_URL=https://tu-backend.onrender.com


Para desarrollo:

VITE_API_URL=http://localhost:4000

4. Cómo ejecutarlo en local

Clonar el repositorio:

git clone https://github.com/BBerasainn/UTN_FINAL_FRONT.git


Instalar dependencias:

npm install


Crear el archivo .env en la raíz del frontend:

VITE_API_URL=http://localhost:4000


Ejecutar el servidor de desarrollo:

npm run dev


- El proyecto quedará disponible en:

http://localhost:5173

5. Flujo de autenticación

El usuario se registra desde el frontend.

El backend envía un email con un enlace de verificación.

El usuario verifica su cuenta a través del token.

Una vez verificado, puede iniciar sesión.

El token se almacena en localStorage.

El usuario accede a la sección privada (chat).

6. Pantallas del proyecto

Login

Register

VerifyAccount

ChatPage
