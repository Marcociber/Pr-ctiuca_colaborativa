# 🔍 Introducción a Nessus: Sistema de Evaluación de Vulnerabilidades

**Nessus** es una de las herramientas más reconocidas en el ámbito de la ciberseguridad para la detección proactiva de vulnerabilidades. Desarrollada por **Tenable, Inc.**, Nessus permite escanear sistemas, redes y dispositivos en busca de debilidades que puedan ser explotadas por atacantes. Es ampliamente utilizada en auditorías de seguridad, pentesting y cumplimiento normativo.

---

## ⚙️ ¿Qué ofrece Nessus?

- Escaneo detallado de sistemas operativos, aplicaciones y dispositivos de red
- Detección de vulnerabilidades conocidas, configuraciones erróneas y software obsoleto
- Base de datos actualizada con más de 70,000 plugins de detección
- Informes personalizables con métricas de riesgo y recomendaciones
- Soporte para escaneos autenticados mediante credenciales
- Integración con herramientas como SIEM, gestores de tickets y plataformas DevSecOps

---

## 🧪 Casos de uso comunes

- Evaluación de seguridad en entornos corporativos y gubernamentales
- Pruebas de cumplimiento con normativas como PCI-DSS, HIPAA, ISO 27001
- Validación de parches y configuraciones tras tareas de remediación
- Soporte en procesos de auditoría interna y externa
- Pentesting como parte de ejercicios de hacking ético

---

## 🛠️ Ventajas de usar Nessus

- Alta precisión en la detección de vulnerabilidades
- Interfaz gráfica intuitiva y fácil de usar
- Escalabilidad para entornos pequeños, medianos y grandes
- Actualizaciones constantes de plugins y base de datos de amenazas
- Compatible con múltiples sistemas operativos (Windows, Linux, macOS)
- Soporte profesional disponible en su versión comercial (Nessus Professional)

---

## 💡 Notas adicionales

Nessus forma parte del ecosistema de soluciones de **Tenable**, junto con Tenable.io y Tenable.sc, lo que permite una gestión centralizada de vulnerabilidades en entornos complejos. Aunque Nessus no es de código abierto, su versión gratuita (Nessus Essentials) permite escanear hasta 16 IPs, ideal para laboratorios y entornos de prueba.

---

> 📌 **Recomendación**: Para entornos de producción o auditorías profesionales, considera adquirir una licencia de Nessus Professional para acceder a todas las funcionalidades y soporte técnico.

---

## 🔗 Fuentes

- [Cibersafety: Nessus, herramienta esencial en ciberseguridad](https://cibersafety.com/nessus-herramienta-gestion-vulnerabilidades-ciberseguridad/)
- [Campus Ciberseguridad: ¿Qué es Nessus y para qué sirve?](https://www.campusciberseguridad.com/blog/que-es-nessus-y-para-que-sirve/)
- [Tenable: Página oficial de Nessus Professional](https://es-la.tenable.com/products/nessus/nessus-professional)

---

##  Instalación 

Lo primero que debemos hacer es irnos a la página de instalación de [Nessus-Teenable](https://www.tenable.com/downloads/nessus?loginAttempted=true), donde escogeremos la versión más reciente y hacia que sistema operativo, en mi caso W11:

![Enumeración](../../Assets/nessus/0,1.png)

Donde, una vez instalado, veremos que nos sale este instalador:

![Enumeración](../../Assets/nessus/0,2.png)

Ejecutamos y nos aparecerá la pantalla para instalar el programa, donde damos a siguiente a todo:

![Enumeración](../../Assets/nessus/0,3.png)

Una vez instalado, nos saldrá en nuestro navegador donde tendremos que registrarnos:

![Enumeración](../../Assets/nessus/1.png)

Le damos directamente a continuar y le damos a `register for Nessus Essentioals`:

![Enumeración](../../Assets/nessus/2.png)

Damos a continuar y ahora rellenamos con nuestro nombre, apellido y correo electrónico para registrarnos en la aplicación:

![Enumeración](../../Assets/nessus/3.png)

Una vez registrados, le damos a continuar y ahora nos aparece que se nos ha activado la licencia con nuestro identificador correspondiente:

![Enumeración](../../Assets/nessus/4.png)

Una vez dado a continuar, tendremos que poner un nombre se usuario y una contraseña:

![Enumeración](../../Assets/nessus/5.png)

Una vez creada la cuenta, veremos que se está inicializando la aplicación, donde está cargando todos los datos para que funcione. suele tardar un poco.

![Enumeración](../../Assets/nessus/6.png)

---

##  Configuración 

Una vez realizada la instalación, nos saldrá la página de inicio, donde directamente sale una ventana donde nos da una pequeña explicación de bienvenida. En la opción `Target`, pondremos nuestro rango de red en la que estemos conectados:

![Enumeración](../../Assets/nessus/7.png)

Una vez dado a continuar, veremos que está haciendo un escaneo de red, detectando las diferentes direcciones que se encuentran activas:

![Enumeración](../../Assets/nessus/8.png)

Una vez realiazo el escaneo, veremos que nos sale nustro escaneo, donde vemos a la derecha que está parado:

![Enumeración](../../Assets/nessus/9.png)

Le damos a iniciar y veremos que empieza el escaneo hacia ese proyecto, donde hace escaneos a las direcciones que ha encontrado:

![Enumeración](../../Assets/nessus/10.png)

Vemos (mientra escanea o ya ha terminado el escaneo), que va analizando las máquinas donde podemos ver a la derecha que hay un gráfico donde nos indica el nivel de peligrosidad de las vulnerabilidades:

![Enumeración](../../Assets/nessus/11.png)

Si nos metemos al escaneo de la dirección 10.224.60.246, vemos al principio la información general de lo que tiene:

![Enumeración](../../Assets/nessus/12.png)

---

##  Uso de herramientas de Nessus

Si damos, arriba a la derecha, al botón de `new scan`, veremos que nos muestra un catálogo de diferentes herramientas que ayudadn a afinar más a la hora de hacer identificación de vulnerabilidades:

![Enumeración](../../Assets/nessus/13.png)

En este caso, vamos a usar la herramienta `Advanced Scan`, permite realizar escaneos altamente configurables y personalizados, ideales para profesionales que necesitan un control granular sobre cómo se ejecutan los análisis de vulnerabilidades.
Donde le nombro como "prueba", pongo una breve descripción y pongo hacia la dirección a escanear:

![Enumeración](../../Assets/nessus/14.png)

En el apartado de `Discovery`, apagamos la opción de `Remote Host Ping`, ya que tenemos la dirección ip encontrada:

![Enumeración](../../Assets/nessus/15.png)

En la sección de puertos, lo dejamos a default, para que haga el escaneo hacia los puertos por defecto:

![Enumeración](../../Assets/nessus/0,6.png)

En el apartado de `Assesment`, vemos que se pueden configurar hacia fuerzas brutas, aplicaciones web, malwares, bases de datos:

![Enumeración](../../Assets/nessus/17.png)

![Enumeración](../../Assets/nessus/18.png)

![Enumeración](../../Assets/nessus/19.png)

En la herramienta, en la sección de `Credentials`, podemos ver que se puede configurar las credenciales, por si se puede añadir:

![Enumeración](../../Assets/nessus/20.png)

En la sección de `Plugins`, podemos ver todos los plugins que tiene para añadir:

![Enumeración](../../Assets/nessus/21.png)

Una vez configurado todo, le damos a `Scan` y vemos que empieza a hacer el escaneo hacia la dirección de red donde empieza el escaneo de vulnerabilidades:

![Enumeración](../../Assets/nessus/22.png)

Una vez terminado el escaneo, podemos ver quie nos saca las vulnerabilidades hacia los puertos asociados, con su correspondiente nombre de vulnerabilidad:

![Enumeración](../../Assets/nessus/24.png)

