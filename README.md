# CoreAI-Plataforma-de-Soporte-Inteligente
📝 Descripción
Este proyecto es una plataforma full-stack diseñada para la automatización de la atención al cliente mediante IA. El sistema permite la creación de tickets, la gestión de estados y la clasificación automática de problemas técnicos mediante la integración de LLMs, optimizando los tiempos de respuesta del equipo de soporte.

🚀 Tecnologías Principales
Frontend: React.js con Axios para comunicación con la API.

Backend: FastAPI (Python) para la gestión de lógica, autenticación y base de datos.

IA/Automatización: n8n para la orquestación de flujos de IA (Gemini API).

Infraestructura: Docker y Docker Compose para el despliegue de microservicios.

Base de Datos: PostgreSQL (mediante SQLAlchemy ORM).

🏗️ Arquitectura del Sistema
El sistema está diseñado bajo un enfoque de microservicios, donde el frontend y el backend se comunican mediante una API RESTful, mientras que el orquestador n8n actúa como un puente inteligente para el procesamiento de lenguaje natural.

⚙️ Configuración e Instalación
Para ejecutar el proyecto en tu entorno local, asegúrate de tener instalado Docker y Docker Compose.

Clonar el repositorio:

Bash
git clone https://github.com/tu-usuario/tu-proyecto.git
cd tu-proyecto
Variables de Entorno:
Crea un archivo .env en la raíz basado en el ejemplo:

Fragmento de código
DATABASE_URL=postgresql://usuario:password@db:5432/soporte_db
# Otras variables necesarias
Ejecutar el sistema:

Bash
docker-compose up -d --build
Acceso:

Frontend: http://localhost:5173

Backend API: http://localhost:8000

✨ Funcionalidades Destacadas
Autenticación Segura: Implementación de JWT para proteger rutas sensibles.

Inteligencia Artificial: Clasificación automática de tickets (prioridad, categoría y diagnóstico) usando IA.

Persistencia de Datos: Arquitectura de volúmenes en Docker para asegurar que los flujos de n8n y la base de datos no se pierdan.

📁 Estructura del Repositorio
Plaintext
/backend          # API FastAPI y lógica de negocio
/frontend         # Interfaz React
/n8n_backup       # Flujos de trabajo de n8n para importar
docker-compose.yml # Orquestación de servicios
🤝 Contribuciones
Este proyecto es parte de mi portafolio. Si tienes sugerencias o mejoras, eres bienvenido a abrir un Issue o Pull Request.
