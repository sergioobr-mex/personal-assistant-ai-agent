# Personal Assistant — AI Agent with Python & Google ADK

## 📌 Descripción

**Personal Assistant** es un agente inteligente desarrollado con **Python y Google Agent Development Kit (ADK)** como proyecto práctico de aprendizaje en Inteligencia Artificial Generativa y desarrollo de agentes.

El objetivo del proyecto es implementar y comprender la estructura fundamental de un agente basado en un modelo de lenguaje (LLM), definiendo su identidad, propósito e instrucciones de comportamiento.

Este proyecto representa el primer nivel de una ruta de desarrollo hacia soluciones más avanzadas de **AI & Data Engineering**, incluyendo posteriormente herramientas, integración con APIs, RAG, embeddings, MCP y bases de datos vectoriales.

---

## 🎯 Objetivo

Construir un agente conversacional básico capaz de responder preguntas utilizando un modelo de lenguaje, aplicando una configuración estructurada mediante Google ADK.

El proyecto busca demostrar conocimientos prácticos en:

* Python aplicado a Inteligencia Artificial.
* Desarrollo básico de agentes.
* Integración con modelos de lenguaje.
* Configuración de agentes mediante Google ADK.
* Diseño de instrucciones para LLMs.
* Organización y documentación de proyectos de IA.

---

## 🏗️ Arquitectura

La arquitectura inicial del proyecto es deliberadamente sencilla:

```text
┌───────────────────────┐
│        Usuario       │
└───────────┬───────────┘
            │
            ▼
┌───────────────────────┐
│      AI Agent         │
│    Google ADK         │
└───────────┬───────────┘
            │
            ▼
┌───────────────────────┐
│    Gemini LLM         │
└───────────────────────┘
```

### Flujo

```text
Usuario
   ↓
Agent
   ↓
Google ADK
   ↓
Gemini
   ↓
Respuesta
```

---

## 🧠 Configuración del agente

El agente se define mediante los siguientes elementos:

* **Model:** modelo de lenguaje utilizado por el agente.
* **Name:** identificador del agente.
* **Description:** descripción de su propósito.
* **Instruction:** instrucciones que determinan su comportamiento y estilo de respuesta.

La implementación se encuentra en:

```text
agent.py
```

---

## 🛠️ Tecnologías

| Tecnología         | Uso                   |
| ------------------ | --------------------- |
| Python             | Lenguaje principal    |
| Google ADK         | Desarrollo del agente |
| Gemini             | Modelo de lenguaje    |
| Git                | Control de versiones  |
| Google Cloud Shell | Entorno de desarrollo |

### Dependencia principal

```text
google-adk==2.6.2
```

---

## 📂 Estructura del proyecto

```text
personal-assistant/
│
├── agent.py
├── __init__.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

> El entorno virtual `.venv` se utiliza únicamente para desarrollo local y no debe incluirse en el repositorio.

---

## ⚙️ Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/sergioobr-mex/personal-assistant-ai-agent.git
personal-assistant-ai-agent
```

### 2. Crear un entorno virtual

```bash
python -m venv .venv
```

### 3. Activar el entorno virtual

Linux / macOS:

```bash
source .venv/bin/activate
```

Windows:

```bash
.venv\Scripts\activate
```

### 4. Instalar dependencias

```bash
pip install -r requirements.txt
```

---

## 🔐 Variables de entorno

Las credenciales y claves privadas no deben almacenarse directamente en el repositorio.

Para configurar las variables necesarias, utilizar:

```text
.env
```

El archivo:

```text
.env.example
```

sirve como referencia para otros desarrolladores.

**Nunca subir claves API, credenciales o secretos al repositorio.**

---

## ▶️ Ejecución

El agente puede ejecutarse utilizando el entorno configurado con Google ADK.

La implementación principal se encuentra en:

```text
agent.py
```

---

## 💬 Ejemplo conceptual

El agente está diseñado para recibir preguntas del usuario y responder utilizando el modelo de lenguaje configurado.

Ejemplo:

```text
Usuario:
¿Qué es un proceso de negocio?

Agent:
Un proceso de negocio es un conjunto estructurado de actividades
que permite transformar entradas en resultados para alcanzar un
objetivo determinado dentro de una organización.
```

---

## 📚 Conceptos aplicados

Este proyecto permitió trabajar los fundamentos de:

### 1. AI Agents

Comprensión de la estructura básica de un agente y su interacción con un modelo de lenguaje.

### 2. Large Language Models

Uso de un LLM como motor de generación de respuestas.

### 3. Prompt / Instruction Engineering

Definición de instrucciones para establecer el comportamiento, contexto y estilo de respuesta del agente.

### 4. Google ADK

Uso del Agent Development Kit para estructurar y configurar un agente basado en IA.

### 5. Python for AI

Aplicación de Python como lenguaje de implementación para soluciones de Inteligencia Artificial.

---

## ⚠️ Limitaciones actuales

Este proyecto representa una implementación inicial y deliberadamente no incluye todavía:

* Retrieval-Augmented Generation (RAG).
* Embeddings.
* Vector databases.
* Model Context Protocol (MCP).
* Herramientas externas.
* Integración con APIs empresariales.
* Persistencia avanzada de información.
* Pipelines de datos.
* Machine Learning supervisado.

Estas capacidades forman parte de la evolución prevista del portafolio.

---
## 🎥 Demo

Video demostrativo de la ejecución e interacción con el agente desarrollado con Python y Google ADK.

[▶️ Ver demostración del agente](./demo/demo-personal-assistant.mp4)

## 🚀 Próxima evolución

El siguiente proyecto llevará la arquitectura hacia un agente más completo incorporando capacidades como:

```text
                    ┌──────────────┐
                    │     Agent    │
                    └──────┬───────┘
                           │
              ┌────────────┼────────────┐
              ▼            ▼            ▼
           Tools          RAG          MCP
              │            │            │
              ▼            ▼            ▼
            APIs      Embeddings    External
                         │           Context
                         ▼
                  Vector Database
```

El objetivo será demostrar cómo evolucionar desde un agente conversacional básico hacia una solución de IA capaz de utilizar conocimiento externo, herramientas e integraciones.

---

## 👨‍💻 Autor

**Sergio Obregón Rosales**

Ingeniero en Sistemas Computacionales | Business & Solution Analysis | AI & Data Engineering

Este proyecto forma parte de mi transición y especialización práctica hacia **AI & Data Engineering**, combinando experiencia previa en análisis de negocio, desarrollo, bases de datos, integración de sistemas y diseño de soluciones con nuevas capacidades en Inteligencia Artificial y Machine Learning.
