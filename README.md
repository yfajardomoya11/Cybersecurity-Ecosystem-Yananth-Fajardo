# 🛡️ Cybersecurity Ecosystem | Integrated SOC Platform
### Developed by **Yananth Fajardo Moya** — `@yfajardomoya11`

> **Un ecosistema de seguridad modular de alto rendimiento diseñado para la automatización de infraestructura, detección proactiva de intrusiones y análisis de inteligencia de amenazas.**

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Security Focus](https://img.shields.io/badge/Focus-Cybersecurity%20%7C%20Blue%20Team-blue?style=for-the-badge)
![Network Automation](https://img.shields.io/badge/Network-Automation-orange?style=for-the-badge)

---

## ⚖️ Legal & Ethical Disclaimer
> [!CAUTION]
> **Aviso de Responsabilidad Profesional** > Este ecosistema ha sido íntegramente desarrollado por **Yananth Fajardo Moya** con fines estrictamente educativos y de investigación en ciberseguridad. 
>
> 1. **Uso Ético:** Las herramientas aquí contenidas deben ser utilizadas únicamente en entornos controlados, laboratorios de seguridad o bajo autorización explícita del propietario de la red (Pentesting Ético).
> 2. **Sin Garantías:** El autor no se responsabiliza por daños, interrupciones de servicio o uso ilícito de este software en infraestructuras de terceros. 
> 3. **Legislación:** El uso de estas herramientas para actividades no autorizadas puede ser penalizado bajo las leyes de delitos informáticos locales e internacionales. 
>
> **La ciberseguridad es una responsabilidad. Úsala para proteger, no para comprometer.**

---

## 🧠 Arquitectura del Sistema (Mini SIEM)

Esta arquitectura simula el flujo de datos de un **Security Operations Center (SOC)** real, optimizando la visibilidad del tráfico y la respuesta ante incidentes.

```mermaid
graph TD
    subgraph "Control & Management"
    A[🌐 Network Security Tool] -->|Push Config| B(Network Devices)
    B -->|Configuration State| A
    end

    subgraph "Detection & Monitoring"
    C[🚨 Sentinel Watch IDS] -->|Packet Inspection| B
    C -->|Alert Stream| E{🛡️ Guardian Engine}
    B -->|Log Aggregation| E
    end

    subgraph "Orchestration & Analysis"
    E -->|Correlation| F[Security Analyst]
    E -.->|Incident Response| A
    end

    style E fill:#1a237e,stroke:#fff,stroke-width:2px,color:#fff
    style A fill:#1b5e20,color:#fff
    style C fill:#b71c1c,color:#fff
    style E fill:#1f425f,stroke:#333,stroke-width:2px,color:#fff
    style A fill:#2e7d32,color:#fff
    style C fill:#c62828,color:#fff


