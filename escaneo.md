## 1. Nmap – Reconocimiento de Red

### ¿Qué es?

Herramienta de línea de comandos para descubrir hosts, puertos abiertos, servicios y sistemas operativos.

### Instalación (Debian/Ubuntu | WSL | macOS Homebrew)

```bash
sudo apt install nmap        # Debian/Ubuntu/WSL
brew install nmap            # macOS Homebrew
```

### Comandos Básicos

| Objetivo                            | Comando                           |
| ----------------------------------- | --------------------------------- |
| Escanear puertos comunes            | `nmap 192.168.1.1`                |
| Escanear **todos** los puertos      | `nmap -p- 192.168.1.1`            |
| Detectar versiones de servicios     | `nmap -sV 192.168.1.1`            |
| Detectar sistema operativo          | `nmap -O 192.168.1.1`             |
| Escaneo agresivo (SYN, versión, SO) | `nmap -sS -sV -O -T4 192.168.1.1` |
| Descubrir hosts en una red /24      | `nmap -sn 192.168.1.0/24`         |

> 💡 Exporta resultados con `-oN salida.txt` (normal) o `-oX salida.xml` (XML).

---

## 2. Nessus – Escáner Comercial (Essentials gratuito)

### ¿Qué es?

Escáner de vulnerabilidades CVE y configuraciones inseguras con interfaz web.

### Instalación y Primer Uso

1. Descarga el paquete apropiado desde [https://www.tenable.com/products/nessus](https://www.tenable.com/products/nessus).
2. Instala y levanta el servicio; accede en tu navegador a `https://localhost:8834`.
3. Registra una licencia **Nessus Essentials** (gratuita para 16 IPs).
4. Crea un **Basic Network Scan** indicando las IP/rangos objetivo.
5. Ejecuta el escaneo y revisa resultados ↠ exporta en PDF/CSV.

### Ventajas Clave

* Clasificación por severidad (Crítico, Alto, Medio…).
* Recomendaciones detalladas y gráficos ejecutivos.

---

## 3. OpenVAS (Greenbone) – Alternativa Open Source

### ¿Qué es?

Plataforma libre para escaneo profundo de vulnerabilidades, similar a Nessus.

### Instalación Rápida (Debian/Kali)

```bash
sudo apt install openvas        # instala dependencias
sudo gvm-setup                  # inicializa base de datos y certificados
sudo gvm-start                  # arranca servicios GVM/OpenVAS
```

> Verifica la instalación con `sudo gvm-check-setup`.

### Uso Básico

1. Accede a `https://localhost:9392` con las credenciales generadas.
2. Actualiza los feeds (NVTs, CERT, SCAP).
3. Crea un **Target** con IPs/rangos.
4. Configura un **Task** usando la policy "Full and Fast".
5. Ejecuta el escaneo y revisa el dashboard de resultados (CVEs, Hosts, Port List).

### Ventajas Clave

* 100 % libre y mantenido por la comunidad.
* Reportes detallados exportables en PDF/HTML/CSV.

---

## 4. ¿Qué Herramienta Elegir?

| Herramienta | Mejor Para                                | Licencia                      |
| ----------- | ----------------------------------------- | ----------------------------- |
| **Nmap**    | Reconocimiento rápido de red              | Open Source                   |
| **Nessus**  | Auditorías con reportes ejecutivos listos | Comercial (Essentials gratis) |
| **OpenVAS** | Escaneos profundos sin costo de licencia  | Open Source                   |

---

## 5. Buenas Prácticas

* Ejecuta Nmap primero para identificar superficies de ataque.
* Realiza escaneos Nessus/OpenVAS fuera de horas pico: son intensivos en red.
* Mantén ambas bases de vulnerabilidades **actualizadas**.
* Valida resultados falsos positivos comparándolos con manuales del proveedor.
* Integra los hallazgos críticos en tu **plan de remediación**.

---
