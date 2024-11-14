## README - Backend

# Sistema de Turnos para Peluquería - Backend

### Descripción del Proyecto

Este es el backend del sistema de turnos para peluquería, encargado de gestionar la creación, cancelación y consulta de turnos, así como el registro de usuarios y el envío de notificaciones por correo electrónico.

---

### Configuración de la Base de Datos

- **Días Laborales**: Lunes a viernes, de 9 a 18 horas. Cada turno tiene una duración máxima de 30 minutos.
- **Restricciones**:
   - No se permite reservar más de un turno en el mismo horario.
   - Cancelación de turnos permitida hasta un día antes de la cita.

---

### Funcionalidades del Backend

1. **Gestión de Turnos**
   - Reservar un turno: Envía confirmación por correo electrónico al usuario.
   - Cancelar turno: Permite cancelar hasta un día antes, y envía una notificación por email.

2. **Manejo de Usuarios**
   - Creación de cuenta: Envía confirmación por correo al registrarse.
   - Inicio de sesión y cierre de sesión.

3. **Carga de Imagen de Perfil**
   - Permite que el usuario suba una foto de perfil en formatos `.jpg`, `.png`, etc., utilizando **Cloudinary**.

---

### User Stories

#### Usuario Invitado
1. Visualizar información básica en la Landing y la página principal (Home).
2. Registrarse y recibir un email de confirmación.

#### Usuario Registrado
1. Iniciar sesión / Cerrar sesión.
2. Reservar un turno dentro del horario laboral y recibir un email de confirmación.
3. Ver historial de turnos.
4. Cancelar turno (hasta un día antes).

---

### Dependencias y Tecnologías

- **Node.js** y **Express** para la lógica de servidor.
- **NodeMailer** para el envío de emails de confirmación.
- **Cloudinary** para la carga y almacenamiento de imágenes de perfil.

---

### Instalación y Ejecución

1. Clonar el repositorio.
2. Instalar dependencias:
   ```bash
   npm install
   ```
3. Configurar variables de entorno:
   - **NodeMailer**: Configuración para envío de emails.
   - **Cloudinary**: Credenciales para la carga de imágenes.
4. Iniciar el servidor:
   ```bash
   npm start
   ```

---

