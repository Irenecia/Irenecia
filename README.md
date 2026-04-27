#Proyecto Final: BOHR, Gestion de Proyectos


> Un sistema integral de gestión empresarial que permite administrar proyectos, tareas y departamentos. Construido con una arquitectura Full Stack moderna.

Este proyecto destaca por su capacidad de gestionar flujos de trabajo complejos, integrando un backend en Python con una interfaz interactiva en React.


### Frontend
*   **Framework:** React 18 con **Vite** para un rendimiento óptimo.
*   **Routing:** React Router Dom v6.
*   **UI & Componentes:** Lucide React (iconos), Lottie (animaciones).
*   **Utilidades:** React Toastify (notificaciones) y FormKit Drag-and-Drop.

### Backend
*   **Lenguaje:** Python.
*   **Arquitectura:** API RESTful organizada por modelos (`User`, `Project`, `Task`, `Department`).
*   **Base de Datos:** SQLAlchemy (ORM) con sistema de migraciones.

## 📂 Estructura del Proyecto

### 💻 Frontend (`/src`)
*   `components/`: Componentes modulares como `ConfirmModal`, `Sidebar`, y formularios dinámicos.
*   `pages/`: Vistas principales incluyendo **Dashboard**, **Login**, **UserProfile** y gestión de contraseñas.
*   `hooks/`: Lógica reutilizable para el estado de la aplicación.
*   `store/`: Manejo del estado global mediante `flux.js`.

### ⚙️ Backend (`/api`)
*   `models.py`: Definición de la estructura de datos (Usuarios, Tareas, Proyectos).
*   `admin.py`: Panel de administración configurado.
*   `commands.py`: Scripts personalizados para la gestión de la base de datos.

## ✨ Funcionalidades Clave
*   **Autenticación Completa:** Registro, Login y recuperación de contraseña segura.
*   **Gestión Jerárquica:** Administración de Departamentos -> Proyectos -> Tareas.
*   **Interfaz Dinámica:** Sistema de arrastrar y soltar para tareas y feedback visual con animaciones.
*   **Panel de Administración:** Gestión de datos desde el backend integrada.

## 🚀 Instalación y Uso

### 1. Clonar y preparar el entorno
```bash
git clone https://github.com
cd nombre-del-repo
```

### 2. Configurar el Backend (Python)
```bash
pip install -r requirements.txt
python manage.py upgrade  # Para las migraciones
python manage.py runserver
```

### 3. Configurar el Frontend (React)
```bash
npm install
npm run dev
```
