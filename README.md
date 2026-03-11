# Sistema Predictor de Riesgo Vial - TFI Grupo 7

Este repositorio centraliza el **Trabajo Final Integrador** para la *Diplomatura en Soluciones Basadas en Inteligencia Artificial (2026)*. El proyecto consiste en una solución tecnológica diseñada para estimar probabilidades de riesgo de accidentes viales basándose en condiciones operativas y climáticas en tiempo real.

## 📋 Descripción del Proyecto

El sistema surge de la necesidad de organismos de seguridad vial y operadores de infraestructura de contar con herramientas preventivas. Utiliza un modelo de Machine Learning para procesar variables como el clima, el tipo de camino, el momento del día y el estado del tránsito, permitiendo una toma de decisiones estratégica y la optimización de recursos en rutas concesionadas.

### Características principales:
- **Predicción en tiempo real:** Estimación de riesgo mediante un modelo de inteligencia artificial optimizado.
- **Panel de Operador:** Interfaz intuitiva para la carga de condiciones y visualización de alertas.
- **Visualización Geoespacial:** Integración de mapas con capas meteorológicas en vivo.
- **Infraestructura Segura:** Despliegue basado en aislamiento por celdas (Jails) en FreeBSD.

---

## 🏗️ Arquitectura del Sistema

El proyecto está dividido en dos componentes principales que se comunican de forma asincrónica:

<img width="2088" height="707" alt="imagen" src="https://github.com/user-attachments/assets/3fbd92df-f831-4e81-97a9-8a6139404419" />


### 1. Backend (Motor de Inferencia)
Desarrollado en **Rust**, se encarga de la lógica de negocio y la ejecución del modelo de IA en formato ONNX. 
* **Repositorio:** [josejachuf/predictor-accidentes](https://github.com/josejachuf/predictor-accidentes)

### 2. Frontend (Interfaz de Usuario)
Desarrollado con **Vue.js** y **Quasar Framework**, ofrece una experiencia de usuario reactiva y adaptable (SPA).
* **Repositorio:** [josejachuf/diplo-tfi-g7-front](https://github.com/josejachuf/diplo-tfi-g7-front)

---

## 🚀 Despliegue Técnico

La solución está diseñada para ejecutarse en entornos de alta disponibilidad y seguridad:
- **OS:** FreeBSD.
- **Contenedores:** Jails administradas mediante **Bastille**.
- **Servidor Web:** Nginx actuando como Proxy Inverso.
- **Modelo:** Inferencia nativa mediante la librería `tract` (sin dependencia de Python en producción).
* **Repositorio:** [josejachuf/diplo-tfi-g7-bastille](https://github.com/josejachuf/diplo-tfi-g7-bastille)


---

## 👥 Integrantes del Grupo 7

- **Alcides Cagna**
- **Diego Garrido**
- **Fernando José Jachuf**
- **Macarena Bressán**
- **Silvia Mabel Espinosa**

**Tutor:** Aybar Lourdes

---

## 📄 Documentación

https://drive.google.com/drive/folders/12ZBgWGgOrYC3WO-prEwVIMm3nmMWauvU
