# Aplicacion de Notas

##  Descripción  
**Aplicacion de notas** es una aplicación web que permite crear, guardar y gestionar tareas y notas de forma sencilla. Cada usuario inicia sesión con un PIN de 4 dígitos, que actúa como clave para su espacio personal en **Firebase Firestore**. Incluye:

- Interfaz responsive (móvil y escritorio)  
- Modo claro/oscuro  
- Animaciones “ripple” en botones  
- Guardado y recuperación de datos en la nube  

---

##  Características principales

-  **Login con PIN**: cada PIN genera o recupera tu colección de tareas y notas.  
-  **Notas especiales**: título + cuerpo de nota “fijada” en la parte superior.  
-  **Gestión de tareas**: agregar, completar y eliminar tareas individuales o todas a la vez.  
-  **Modo claro/oscuro**: alterna theme sin recargar la página.  
-  **Persistencia en Firebase**: datos guardados en Firestore bajo la colección `lists/<PIN>`.  

---

##  Capturas de pantalla  

<div align="center">  
  <img src="screenshots/login.png" alt="Pantalla de login con PIN" width="300" />  
  &nbsp;&nbsp;  
  <img src="screenshots/main.png" alt="Vista principal con tareas y notas" width="300" />  
</div>  

---

## Tecnologías utilizadas

- **HTML5** + **CSS3** (Mobile‑first, variables CSS, media queries)  
- **JavaScript** (ES6+, módulos, jQuery para animaciones)  
- **Firebase**  
  - `firebase-app-compat.js`  
  - `firebase-firestore-compat.js`  
- **Ionicons** (v5) para iconografía  
- **Ripple effect** (script personalizado)  

---

##  Instalación y despliegue

1. **Clona el repositorio**  
   ```bash
   git clone https://github.com/TU_USUARIO/Aplicaci-n-de-Listas.git
   cd Aplicacion-de-Listas
   ```
##  Configura Firebase

- Crea un proyecto y app web en Firebase Console.
- Habilita Cloud Firestore en modo "test".
- Copia tu bloque `firebaseConfig` en `script.js` (reemplaza los `"<-->"`).

## Abre la app

No hace falta servidor: abre `index.html` en tu navegador.

Introduce un PIN de 4 dígitos y haz clic en **Continuar**.

## Despliega (opcional)

Puedes usar GitHub Pages, Netlify o Vercel:

- Configura el build (si usas bundler) o publica directamente la carpeta raíz.

## Uso

- **Login**: introduce tu PIN y continúa.
- **Editar nombre**: haz clic en _"¡Bienvenido, [Nombre]!"_ para cambiarlo.
- **Crear nota**: pulsa _"Nota especial"_ o en el menú lateral → escribe título y texto → **Guardar**.
- **Añadir tarea**: pulsa _"Agregar tarea"_ → completa campos → **Guardar**.
- **Eliminar tarea**: clic en _"X"_ en la tarjeta o _"🗑️"_ junto a _"Tareas"_ para eliminarlas todas.
- **Cambiar tema**: menú lateral → _"Cambiar tema"_.
- **Cerrar sesión**: menú lateral → _"Cerrar sesión"_ para volver al login.

## Contribuciones

¡Bienvenidas! Si quieres aportar:

1. Haz un fork del repositorio.
2. Crea una rama: `git checkout -b feature/mi-nueva-funcionalidad`.
3. Haz tus cambios y commit: `git commit -m "feat: añade función X"`.
4. Push a tu fork: `git push origin feature/mi-nueva-funcionalidad`.
5. Abre un **Pull Request** y describe tu propuesta.
