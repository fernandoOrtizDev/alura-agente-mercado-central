# 🛒 Asistente Virtual - Mercado Central 24h 🤖

Un asistente virtual inteligente desarrollado en **Python**, **Streamlit** y la API oficial de **Google Gemini**, diseñado para automatizar la atención al cliente y resolver consultas frecuentes sobre políticas de devoluciones, horarios y productos de forma instantánea. El proyecto está alojado en una infraestructura escalable en la nube bajo un enfoque modular y optimizado.

---

## 📋 Descripción General del Proyecto

El **Asistente Virtual de Mercado Central 24h** surge como una solución tecnológica para optimizar los canales de atención al cliente de un comercio minorista que opera de forma continua. Utilizando Modelos de Lenguaje Grande (LLMs) de última generación, el agente es capaz de interpretar solicitudes en lenguaje natural, comprender el contexto de la conversación y brindar respuestas precisas alineadas estrictamente con las políticas comerciales internas de la tienda, reduciendo la carga operativa del personal humano y mejorando la satisfacción del usuario final.

---
---

## 📺 Capturas de Ejecución en Entornos

### 1. Ejecución en Google Colab
<img width="1450" height="794" alt="Captura de pantalla 2026-07-27 a la(s) 8 39 49 p m" src="https://github.com/user-attachments/assets/e83fa284-338a-49f7-b762-cf64a94e312d" />


### 2. Ejecución en Servidor Cloud (Oracle VM Ubuntu)
<img width="1420" height="825" alt="Captura de pantalla 2026-07-27 a la(s) 11 08 07 p m" src="https://github.com/user-attachments/assets/17219ee3-4018-41ec-b8a7-217a3e83b467" />


---
---

## 📐 Arquitectura de la Solución Implementada

El sistema se estructura bajo una arquitectura cliente-servidor orientada a componentes web interactivos:

1. **Capa de Presentación (Interfaz de Usuario):** Desarrollada con **Streamlit**, maneja de forma eficiente el estado de la sesión (`st.session_state`) para renderizar un historial de chat dinámico, responsivo y en tiempo real para cada usuario.
2. **Capa de Lógica e Inteligencia Artificial:** Emplea el SDK oficial de **Google GenAI** (`google-genai`), conectándose al modelo **Gemini 1.5 Flash**. Se le inyectan directrices institucionales del negocio (`SYSTEM_INSTRUCTION`) para restringir el comportamiento del modelo y asegurar la veracidad de la información comercial suministrada.
3. **Capa de Infraestructura y Despliegue:** Se ejecuta en un servidor Linux (Ubuntu) alojado en la nube, con gestión segura de credenciales mediante variables de entorno y exposición controlada de puertos a través del servidor web integrado de Streamlit.

---

## 🛠️ Tecnologías y Herramientas Utilizadas

<h4>Core Technologies</h4>
<span>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" title="Python">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" title="Streamlit">
  <img src="https://img.shields.io/badge/Google_Gemini-8E75B2?style=for-the-badge&logo=google&logoColor=white" title="Google Gemini">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" title="Linux Ubuntu">
</span>

<h4>Infrastructure & Tools</h4>
<span>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" title="Git">
  <img src="https://img.shields.io/badge/SSH-121011?style=for-the-badge&logo=gnu-bash&logoColor=white" title="SSH">
  <img src="https://img.shields.io/badge/Pip-3776AB?style=for-the-badge&logo=pypi&logoColor=white" title="Python Pip">
</span>

---

## 💻 Instrucciones para Ejecutar el Proyecto

### Prerrequisitos
* Tener instalado **Python 3.8+** y pip en tu entorno local o servidor.
* Contar con una API Key válida de Google AI Studio (`GOOGLE_API_KEY`).

### Pasos de Instalación y Puesta en Marcha

1. Clona el repositorio e ingresa al directorio del proyecto:
   ```bash
   git clone [https://github.com/fernandoOrtizDev/alura-agente-mercado-central.git](https://github.com/fernandoOrtizDev/alura-agente-mercado-central.git)
   cd alura-agente-mercado-central
