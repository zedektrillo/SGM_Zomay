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
