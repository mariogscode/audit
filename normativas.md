# 🛡️ Estándares de Cumplimiento en Ciberseguridad

Este documento detalla los principales **estándares internacionales y regulaciones** que se deben evaluar durante una auditoría de seguridad, especialmente en organizaciones que manejan información sensible, datos personales, financieros o médicos.

---

## 📋 Contenido

1. [ISO/IEC 27001](#isoiec-27001)
2. [PCI DSS](#pci-dss)
3. [HIPAA](#hipaa)
4. [RGPD / GDPR](#rgpd--gdpr)

---

## 📘 ISO/IEC 27001

**¿Qué es?**  
Norma internacional para establecer un **Sistema de Gestión de Seguridad de la Información (SGSI)**.

**Aplica a:**  
- Organizaciones que quieran proteger la confidencialidad, integridad y disponibilidad de la información.
- Empresas que buscan certificarse internacionalmente.

**Pruebas clave:**
- [ ] Revisión de políticas de seguridad documentadas.
- [ ] Evaluación de gestión de riesgos.
- [ ] Validación de controles de acceso físicos y digitales.
- [ ] Revisión de continuidad del negocio y recuperación ante desastres.
- [ ] Capacitación en seguridad para empleados.

---

## 💳 PCI DSS (Payment Card Industry Data Security Standard)

**¿Qué es?**  
Requisitos mínimos para **proteger datos de tarjetas de crédito y débito**, definidos por las principales marcas (Visa, MasterCard, etc.).

**Aplica a:**  
- Comercios y plataformas que **procesan, almacenan o transmiten datos de pago**.

**Pruebas clave:**
- [ ] Escaneo de red externa por un ASV autorizado.
- [ ] Segmentación de red entre sistemas críticos y de oficina.
- [ ] Validación de cifrado de datos en tránsito y en reposo.
- [ ] Revisar que no se almacenen datos sensibles (como CVV).
- [ ] Revisión de políticas de monitoreo, logs y gestión de accesos.

---

## 🏥 HIPAA (Health Insurance Portability and Accountability Act)

**¿Qué es?**  
Ley estadounidense que regula la **protección de información médica** (PHI).

**Aplica a:**  
- Instituciones de salud, aseguradoras, laboratorios, y terceros que manejen PHI (apps, software médico, etc.).

**Pruebas clave:**
- [ ] Control de acceso lógico a datos de salud.
- [ ] Cifrado de PHI en bases de datos y durante transmisión.
- [ ] Evaluación de políticas de privacidad y consentimiento.
- [ ] Revisión de incidentes anteriores y respuesta a brechas.
- [ ] Validación de auditorías y logs de acceso a datos.

---

## 🇪🇺 RGPD / GDPR (Reglamento General de Protección de Datos)

**¿Qué es?**  
Regulación europea para proteger los **datos personales de los ciudadanos de la UE**.

**Aplica a:**  
- Cualquier empresa que procese datos personales de ciudadanos europeos, sin importar su ubicación geográfica.

**Pruebas clave:**
- [ ] Consentimiento explícito del usuario para el uso de sus datos.
- [ ] Acceso, corrección y eliminación de datos (derechos ARCO).
- [ ] Presencia de un DPO (Data Protection Officer), si aplica.
- [ ] Revisión de políticas de privacidad visibles y actualizadas.
- [ ] Evaluación de almacenamiento mínimo y transferencia internacional de datos.

---

## 📂 Uso en auditorías

Estas normativas pueden evaluarse como parte de un:

- 🧪 **Pentest** especializado (PCI, ISO)
- 📊 **Assessment documental** (GDPR, HIPAA)
- 🧾 **Checklist de cumplimiento** para certificaciones o revisiones internas

---

## 🧑‍💻 Autor
Elaborado por el equipo de ciberseguridad con base en los marcos oficiales de:
- [ISO](https://www.iso.org/isoiec-27001-information-security.html)
- [PCI Security Standards Council](https://www.pcisecuritystandards.org/)
- [HIPAA Guidelines](https://www.hhs.gov/hipaa/)
- [Reglamento GDPR UE](https://gdpr.eu/)

---

