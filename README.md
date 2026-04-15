# SGM-Zomay: Sistema de Gestión para Salón de Eventos

Este proyecto forma parte del desarrollo académico para la materia de Computación en Java. El objetivo es digitalizar y optimizar los procesos operativos del **Salón Zomay**.

---

## Resumen 

### Descripción
El **SGM-Zomay** (Sistema de Gestión de Maniobras Zomay) es una aplicación robusta desarrollada en Java diseñada para centralizar la administración de eventos sociales (aniversarios, XV años, bodas). El sistema permite la gestión de contratos, cronogramas de servicios y coordinación de proveedores en una plataforma única.

### Problema Identificado
Actualmente, el Salón Zomay maneja su logística de forma manual o dispersa, lo que incrementa el riesgo de errores en la programación de servicios críticos (como el banquete o la banda sinaloense) y falta de integridad en los datos de los clientes. Esta desorganización puede afectar la calidad del evento y la satisfacción del cliente.

### Solución
Se implementó una solución de software bajo el paradigma de **Programación Orientada a Objetos (POO)** que automatiza la creación de eventos, valida la disponibilidad de fechas y asegura que todos los servicios contratados estén vinculados a una estructura de datos centralizada (`Evento.java`), eliminando el margen de error humano en los cálculos logísticos.

### Arquitectura
El sistema sigue una arquitectura de capas diseñada para la escalabilidad:
* **Presentación:** Interfaz gráfica desarrollada en NetBeans (JFrame).
* **Lógica de Negocio:** Motor en Java con Maven que gestiona las reglas del salón.
* **Control de Versiones:** Repositorio en GitHub con flujo de ramas (`main`/`develop`).
* **Calidad (CI):** Integración continua mediante GitHub Actions para validación de código.

---

##  Tabla de Contenidos (ToC)

1. [Descripción General](#descripción)
2. [Requerimientos del Sistema](#requerimientos)
3. [Instalación y Configuración](#instalación)
4. [Guía de Uso](#uso)
5. [Documentación Técnica (Wiki)](https://github.com/zedektrillo/SGM_Zomay/wiki)
6. [Roadmap del Proyecto](#roadmap)
7. [Guía de Contribución](#contribución)

   ---

## 2. Requerimientos del Proyecto

Para asegurar el correcto funcionamiento y despliegue del sistema **SGM-Zomay**, se han definido los siguientes estándares técnicos:

### A. Infraestructura y Servidores
* [cite_start]**Servidor de Aplicaciones:** No se requiere un servidor de aplicaciones externo (como Tomcat o GlassFish) debido a que la arquitectura actual es una aplicación de escritorio basada en **Java Swing**. [cite: 31]
* [cite_start]**Servidor Web:** No aplica en esta fase; el acceso es local para el personal administrativo del salón. [cite: 31]
* **Base de Datos:** El sistema está diseñado para integrarse con **MySQL 8.0** en fases posteriores. [cite_start]Actualmente, la persistencia se maneja mediante estructuras de datos en memoria y archivos locales. [cite: 28, 33]

### B. Especificaciones de Software (Stack Tecnológico)
* **Versión de Java:** Java SE Development Kit (JDK) **8 o superior**. [cite_start]Se recomienda JDK 17 para mayor estabilidad. [cite: 32]
* [cite_start]**IDE (Entorno de Desarrollo):** **NetBeans 12.0** o superior para el manejo de formularios JFrame y compilación con Maven. [cite: 31]
* [cite_start]**Gestor de Dependencias:** **Apache Maven**, encargado de gestionar el ciclo de vida del proyecto y las librerías externas. [cite: 32]

### C. Paquetes y Librerías Adicionales
* [cite_start]**JUnit 5:** Utilizado para la automatización de pruebas unitarias que validan la lógica de la clase `Evento.java`. [cite: 26, 34]
* [cite_start]**GitHub Actions:** Implementado como el motor de Integración Continua (CI) para validar que el código sea estable antes de cada commit. [cite: 25, 26, 34]


---

## 3. Instalación

Para poner en marcha el ambiente de desarrollo y ejecutar la solución, siga estos pasos detallados:

### A. Configuración del Ambiente de Desarrollo
1. **Clonación del Repositorio:**
   Abra una terminal y ejecute el siguiente comando para obtener el código fuente:
   ```bash
   git clone [https://github.com/zedektrillo/SGM_Zomay.git](https://github.com/zedektrillo/SGM_Zomay.git)

## Preparación y Ejecución Local

Para validar el funcionamiento del sistema en un entorno local, siga estas instrucciones:

### Compilación con Maven
El proyecto utiliza **Maven** para gestionar el ciclo de vida. Ejecute el siguiente comando en la terminal desde la raíz del proyecto:
```bash
mvn clean compile
