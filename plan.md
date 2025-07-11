# 🛡️ Plan Detallado de Auditoría de Ciberseguridad

## 1. Objetivo del Plan

Evaluar el estado actual de la seguridad de la organización—infraestructura, aplicaciones y procesos—e identificar riesgos, vulnerabilidades y brechas de cumplimiento frente a marcos internacionales (OWASP, ISO 27001, PCI DSS, HIPAA, GDPR).

---

## 2. Fases del Plan

### 🔍 Fase 1 · Alcance y Preparación

**Objetivo:** Definir los sistemas, datos y normativas a auditar.

* Identificación de activos (apps web, APIs, red, nube, endpoints).
* Mapeo de datos sensibles (personales, financieros, médicos).
* Reunión con stakeholders y definición de cronograma.
* Selección de estándares aplicables (OWASP, ISO 27001, PCI DSS, HIPAA, GDPR).

📄 **Entregable:** Documento de Alcance (Statement of Work / Charter).

---

### 🏗️ Fase 2 · Levantamiento de Información

**Objetivo:** Recolectar arquitectura, configuraciones y políticas vigentes.

* Diagramas de red y flujos de datos.
* Inventario de hardware/software y activos cloud.
* Políticas y procedimientos de seguridad.
* Roles y permisos actuales.

📄 **Entregable:** Informe de Inventario y Documentación.

---

### 🧪 Fase 3 · Evaluación Técnica

**Objetivo:** Detectar vulnerabilidades técnicas.

#### 3.1 OWASP Web Security Testing

* Chequeo manual y automático (OWASP Top 10).

#### 3.2 Escaneo de Infraestructura

* Nmap, Nessus/OpenVAS: puertos, versiones, servicios inseguros.

#### 3.3 Pentesting (opcional)

* Ataques simulados sobre red interna/externa, APIs y móviles.

#### 3.4 Seguridad en la Nube

* Revisión IAM, buckets públicos, cifrado, configuraciones erróneas.

📄 **Entregable:** Informe Técnico de Vulnerabilidades con evidencia.

---

### 📋 Fase 4 · Evaluación Normativa y de Cumplimiento

**Objetivo:** Verificar alineación con estándares/regulaciones.

* **ISO 27001:** controles SGSI (Anexo A).
* **PCI DSS:** datos de tarjeta, segmentación, cifrado, monitoreo.
* **HIPAA:** protección y confidencialidad de PHI.
* **GDPR:** consentimiento, derechos ARCO, DPO, retención y transferencias.

📄 **Entregable:** Informe de Cumplimiento y Checklist por normativa.

---

### 🧾 Fase 5 · Informe Final y Plan de Remediación

**Objetivo:** Consolidar hallazgos, clasificar riesgos y proponer acciones.

* Tabla de vulnerabilidades (descripción, riesgo, evidencia, norma asociada).
* Recomendaciones técnicas y de proceso.

📄 **Entregables:**

* Informe Ejecutivo (alta gerencia).
* Informe Técnico (equipo IT).
* Plan de Acción priorizado.

---

### 🔁 Fase 6 · Validación de Remediación (Opcional)

**Objetivo:** Confirmar corrección de hallazgos críticos.

* Re‑ejecución de pruebas sobre vulnerabilidades mitigadas.
* Verificación de políticas/procedimientos actualizados.

📄 **Entregable:** Informe de Validación / Auditoría de Seguimiento.

---

## 3. Cronograma de Referencia

| Fase                  | Duración Estimada |
| --------------------- | ----------------- |
| Alcance y Preparación | 2 días            |
| Levantamiento         | 3 días            |
| Evaluación Técnica    | 5–10 días         |
| Evaluación Normativa  | 3–5 días          |
| Informe & Remediación | 3 días            |
| Validación (opcional) | 1–2 semanas       |

---

## 4. Roles y Responsables

| Rol                           | Responsable                             |
| ----------------------------- | --------------------------------------- |
| Auditor Principal             | Consultor externo / equipo de seguridad |
| Soporte Técnico               | Equipo TI interno                       |
| DPO / Oficial de Cumplimiento | Área legal / datos                      |
| Stakeholder de Negocio        | Dirección / Gerencia                    |

---
