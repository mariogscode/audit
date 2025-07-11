# 🛡️ OWASP Manual Security Testing Checklist

Este repositorio contiene una guía práctica para realizar pruebas manuales de seguridad en aplicaciones web, basadas en el estándar **OWASP Top 10**.

## 🎯 Objetivo
Detectar y documentar vulnerabilidades comunes de seguridad mediante pruebas simples y efectivas que cualquier equipo técnico puede realizar, incluso sin herramientas avanzadas.

---

## ✅ Checklist de pruebas

### 🔐 A01: Broken Access Control
- [ ] Acceder a rutas sin estar autenticado (ej. `/admin`, `/dashboard`)
- [ ] Manipular el ID de recursos para acceder a los de otros usuarios (ej. `/user/2`)
- [ ] Realizar acciones no autorizadas (borrar, editar) con un usuario sin permisos

---

### 🔒 A02: Cryptographic Failures
- [ ] Verificar que el sitio use HTTPS con certificado válido
- [ ] Asegurar que contraseñas no estén en texto plano
- [ ] Revisar atributos de cookies: `Secure`, `HttpOnly`, `SameSite`

---

### 💥 A03: Injection
- [ ] Probar inyecciones SQL con entradas como `' OR '1'='1`
- [ ] Inyectar código malicioso en formularios (ej. XSS: `<script>alert(1)</script>`)
- [ ] Manipular parámetros de formularios o URLs

---

### 🧩 A04: Insecure Design
- [ ] Evaluar funciones críticas sin controles (reset de contraseña, acceso a pagos)
- [ ] Verificar lógica insegura (subida de archivos sin validaciones, flujos mal protegidos)

---

### 🛠 A05: Security Misconfiguration
- [ ] Buscar mensajes de error con información sensible (stack trace, versiones)
- [ ] Verificar acceso a rutas ocultas o de respaldo (`/admin`, `/backup`)
- [ ] Revisar cabeceras de seguridad (CSP, X-Content-Type-Options)

---

### 🔑 A07: Identification and Authentication Failures
- [ ] Validar si permite contraseñas débiles
- [ ] Probar fuerza bruta (sin captcha, sin bloqueo)
- [ ] Revisar si los tokens de sesión pueden reutilizarse o compartirse

---

### 🧬 A08: Software and Data Integrity Failures
- [ ] Verificar librerías JS externas sin etiquetas de integridad (`integrity`)
- [ ] Confirmar validación de integridad en descargas o cargas de datos

---

### 📤 A09: Security Logging and Monitoring Failures
- [ ] Comprobar si los intentos de login fallidos quedan registrados
- [ ] Confirmar si existen alertas por actividades sospechosas
- [ ] Validar que los ataques no pasen desapercibidos

---

### 🌐 A10: Server-Side Request Forgery (SSRF)
- [ ] Probar si el servidor puede hacer requests internos manipulando URLs (ej. `http://localhost`)
- [ ] Detectar si funciones como carga de imágenes o previews permiten atacar la red interna

---

## 🧪 Herramientas recomendadas
- [OWASP ZAP](https://www.zaproxy.org/)
- [Burp Suite Community](https://portswigger.net/burp/community)
- [Postman](https://www.postman.com/)
- Navegador + DevTools (para análisis manual)

---

## 🧾 Resultado esperado
Después de completar esta checklist, deberías tener:
- Evidencia de cada prueba (capturas, respuestas del sistema)
- Vulnerabilidades clasificadas por riesgo
- Recomendaciones para corregir cada hallazgo

---

## 👨‍💻 Autor
Elaborado por el equipo de seguridad o QA para auditorías manuales siguiendo las mejores prácticas del proyecto [OWASP](https://owasp.org).

