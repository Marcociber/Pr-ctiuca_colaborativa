# 🛡️ Introducción a AMASS

**AMASS** (Asset Mapping and Scanning System) es una herramienta de código abierto desarrollada por OWASP para la identificación, mapeo y análisis de activos digitales. Es ampliamente utilizada en ciberseguridad ofensiva y defensiva, ya que permite descubrir dominios, subdominios, direcciones IP y otras superficies de ataque expuestas.

## 🚀 Funcionalidades principales

- Reconocimiento pasivo y activo de dominios
- Enumeración de redes mediante OSINT
- Visualización de relaciones entre activos
- Integración con fuentes como Shodan, VirusTotal, Censys
- Automatización de auditorías de seguridad

## 🔧 Casos de uso

- Evaluación de exposición digital
- Pentesting y simulaciones de ataque
- Monitoreo de infraestructura pública
- Investigación de amenazas

## 📦 Ventajas

- Flexibilidad para distintos entornos
- Comunidad activa
- Integración en flujos de trabajo complejos

---

💡 *AMASS es mantenida por OWASP (Open Worldwide Application Security Project), lo que garantiza su calidad y enfoque en la seguridad.*



## Instalación y configuración:

Para empezar, tendremos que bajarnos el repositorio de amass en github, cuya dirección es [esta](https://github.com/owasp-amass/amass).

En una máquina virtual, preferiblemente kali linux, tendremos que clonar el repositorio en local, con el siguiente comando:


## 📦 Comando para clonar

```bash
git clone https://github.com/owasp-amass/amass.git

```

Una vez instalado, veremos que contiene la carpeta /amass donde dentro incluye:

![Contenido del directorio](../../Assets/image.png)

Para ver la ayuda de la herramienta, tendremos que usar el comando:

```bash
amass -h

```

Donde veremos que incluye toda la información relacionada con la herramienta:

![Contenido del directorio](../../Assets/help.png)
