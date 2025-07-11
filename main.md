# 🔐 Auditoría de Ciberseguridad - Guía de Pruebas Completas

Este repositorio documenta un enfoque integral para la realización de auditorías de seguridad en infraestructuras, aplicaciones web y entornos en la nube, combinando prácticas del estándar OWASP con pruebas adicionales fundamentales.

---

## 🎯 Objetivo

Evaluar el nivel de seguridad de una organización mediante pruebas técnicas y de configuración, identificando vulnerabilidades, malas prácticas y oportunidades de mejora.

---

## 🧪 Áreas de pruebas incluidas

### 1. ✅ OWASP Top 10 (Aplicaciones Web)
Basado en las vulnerabilidades más comunes en desarrollo web.

- A01: Broken Access Control
- A02: Cryptographic Failures
- A03: Injection
- A04: Insecure Design
- A05: Security Misconfiguration
- A07: Identification and Authentication Failures
- A08: Software and Data Integrity Failures
- A09: Logging and Monitoring Failures
- A10: Server-Side Request Forgery (SSRF)

👉 Ver el archivo [`owasp-checklist.md`](./owasp-checklist.md) para detalles prácticos y ejemplos de prueba.

---

### 2. 🖥️ Revisión de Infraestructura
- Escaneo de puertos abiertos (ej. Nmap)
- Revisión de versiones y parches de sistema
- Configuración de firewall, VPN y servicios expuestos
- Validación de políticas de backup y recuperación

---

### 3. 🧬 Análisis de Vulnerabilidades
- Herramientas: Nessus, OpenVAS, Qualys
- Detección de software desactualizado y servicios inseguros

---

### 4. 💣 Pruebas de Penetración (Pentesting)
- Simulación de ataques reales a sistemas internos y externos
- Pruebas manuales y automatizadas (ej. Metasploit, Burp Suite)

---

### 5. ☁️ Evaluación de Seguridad en la Nube
- Revisión de configuraciones en AWS, GCP, Azure
- IAM, permisos, buckets públicos, logging activo

---

### 6. 🛠 Hardening y Configuración
Comparación contra estándares como:

- CIS Benchmarks
- STIG (Defense/DoD)
- Validación de contraseñas, sesiones, antivirus, EDR, etc.

---

### 7. 🎣 Ingeniería Social (opcional y bajo acuerdo)
- Simulación de phishing
- Pruebas de conciencia del usuario

---

### 8. 📊 Revisión de Logs y Monitoreo
- Verificación de registros de eventos críticos
- Alertas y mecanismos de detección de incidentes

---

### 9. 📜 Cumplimiento Normativo
- Revisión contra regulaciones y normas aplicables:
👉 Ver el archivo [`normativas.md`](./normativas.md) para mas informacion.
  - ISO/IEC 27001
  - PCI DSS
  - HIPAA
  - RGPD/GDPR

---

### 10. 🧾 Revisión de Código Fuente (si aplica)
- Búsqueda de contraseñas hardcodeadas
- Validación de entradas
- Dependencias inseguras

---

## 📂 Estructura sugerida del repositorio

