# 🚀 CoreAI - Plataforma Inteligente de Soporte Técnico

> Sistema Full Stack para automatizar la atención al cliente mediante Inteligencia Artificial, clasificación inteligente de tickets y gestión centralizada de incidencias.

![Status](https://img.shields.io/badge/Status-En%20Desarrollo-success)
![React](https://img.shields.io/badge/Frontend-React-blue)
![FastAPI](https://img.shields.io/badge/Backend-FastAPI-green)
![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-blue)
![Docker](https://img.shields.io/badge/Infrastructure-Docker-2496ED)
![n8n](https://img.shields.io/badge/Automation-n8n-orange)

---

## 📌 Descripción General

**CoreAI** es una plataforma diseñada para optimizar los procesos de soporte técnico mediante el uso de Inteligencia Artificial y automatización de flujos de trabajo.

La solución permite registrar solicitudes de soporte, administrar tickets, clasificar incidencias automáticamente y generar diagnósticos preliminares utilizando modelos de lenguaje (LLMs), reduciendo significativamente los tiempos de respuesta y mejorando la experiencia del usuario.

---

## ✨ Características Principales

### 🤖 Clasificación Inteligente de Tickets

* Identificación automática de categorías.
* Asignación de prioridades.
* Generación de diagnósticos preliminares.
* Integración con modelos de IA mediante Gemini.

### 🔐 Autenticación y Seguridad

* Implementación de JWT.
* Protección de rutas privadas.
* Gestión segura de usuarios y sesiones.

### 📋 Gestión de Incidencias

* Creación y seguimiento de tickets.
* Actualización de estados.
* Historial de solicitudes.
* Panel de administración para el equipo de soporte.

### ⚡ Automatización de Procesos

* Flujos automatizados mediante n8n.
* Integración entre IA y backend.
* Procesamiento automático de solicitudes.

### 💾 Persistencia de Datos

* Base de datos PostgreSQL.
* Uso de volúmenes Docker para evitar pérdida de información.
* Respaldo de flujos de automatización.

---

## 🛠️ Stack Tecnológico

| Tecnología     | Uso                       |
| -------------- | ------------------------- |
| React.js       | Frontend                  |
| Axios          | Consumo de APIs           |
| FastAPI        | Backend REST              |
| PostgreSQL     | Base de Datos             |
| SQLAlchemy     | ORM                       |
| n8n            | Automatización e IA       |
| Gemini API     | Procesamiento Inteligente |
| Docker         | Contenedorización         |
| Docker Compose | Orquestación de Servicios |

---

## 🏗️ Arquitectura

```text
┌───────────────┐
│   Frontend    │
│   React.js    │
└───────┬───────┘
        │ HTTP
        ▼
┌───────────────┐
│    FastAPI    │
│    Backend    │
└───────┬───────┘
        │
 ┌──────┴──────────┐
 │                 │
 ▼                 ▼
PostgreSQL      n8n + IA
 Database       Gemini API
```

La arquitectura sigue un enfoque basado en microservicios donde cada componente cumple una responsabilidad específica, permitiendo escalabilidad y mantenimiento eficiente.

---

## 📂 Estructura del Proyecto

```plaintext
CoreAI/
│
├── backend/              # API FastAPI y lógica de negocio
├── frontend/             # Aplicación React
├── n8n_backup/           # Flujos exportados de n8n
├── docker-compose.yml    # Orquestación de servicios
├── .env                  # Variables de entorno
└── README.md
```

---

## ⚙️ Instalación Local

### 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/CoreAI.git

cd CoreAI
```

### 2️⃣ Configurar Variables de Entorno

Crear un archivo `.env`:

```env
DATABASE_URL=postgresql://usuario:password@db:5432/soporte_db

JWT_SECRET_KEY=tu_clave_secreta

GEMINI_API_KEY=tu_api_key
```

---

### 3️⃣ Levantar los servicios

```bash
docker-compose up -d --build
```

---

## 🌐 Acceso a la Aplicación

| Servicio          | URL                        |
| ----------------- | -------------------------- |
| Frontend          | http://localhost:5173      |
| Backend API       | http://localhost:8000      |
| Documentación API | http://localhost:8000/docs |
| n8n               | http://localhost:5678      |

---

## 📸 Capturas de Pantalla

### Dashboard

```md
![Dashboard](./screenshots/dashboard.png)
```

### Gestión de Tickets

```md
![Tickets](./screenshots/tickets.png)
```

### Flujo de IA

```md
![IA](./screenshots/ia-flow.png)
```

---

## 🎯 Objetivos del Proyecto

* Automatizar procesos de soporte técnico.
* Reducir tiempos de respuesta.
* Mejorar la organización de incidencias.
* Implementar soluciones de IA aplicadas a entornos reales.
* Desarrollar una arquitectura escalable basada en microservicios.

---

## 👨‍💻 Autor

**Brayan Steven López Morales**

Proyecto desarrollado como parte de mi portafolio profesional enfocado en desarrollo Full Stack, automatización de procesos e Inteligencia Artificial.

📫 Contacto:

* LinkedIn
* GitHub
* Correo electrónico

---

⭐ Si este proyecto te resulta interesante, no olvides darle una estrella al repositorio.

