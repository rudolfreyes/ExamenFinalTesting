# Reporte de Vulnerabilidades — Carlos

**Fecha:** 2024-12-19  
**Proyecto:** Vulnerable Accounting System  
**Grupo de Testing**

---

## Resumen

Durante el análisis de seguridad del sistema Vulnerable Accounting System, identifiqué y documenté **5 vulnerabilidades de severidad baja** que representan riesgos menores pero importantes para la seguridad del sistema. Estas vulnerabilidades se encuentran en los rangos 41 a 45 y abarcan problemas relacionados con la exposición de rutas de archivos en errores, falta de timeout en sesiones, permisos solo en cliente, falta de validación de contenido XML (XXE) y race conditions con errores de lógica de negocio.

---

## Vulnerabilidades Identificadas

### Vulnerabilidad 41: Exposición de rutas de archivos en errores
**Severidad:** Low

### Vulnerabilidad 42: Falta de timeout en sesiones
**Severidad:** Low

### Vulnerabilidad 43: Permisos solo en cliente
**Severidad:** Low

### Vulnerabilidad 44: Falta de validación de contenido XML (XXE)
**Severidad:** Low

### Vulnerabilidad 45: Race Conditions y Business Logic Flaws
**Severidad:** Low

---

## Mi Contribución al Proyecto

Durante el desarrollo de este proyecto de análisis de seguridad, me enfoqué en la identificación y documentación de vulnerabilidades relacionadas con el manejo de errores, la gestión de sesiones, la validación de permisos y la lógica de negocio. Realicé un análisis exhaustivo de los mensajes de error generados por la aplicación, identificando que se exponían rutas completas del sistema de archivos, lo cual facilitaba la enumeración de la estructura.

Mi trabajo incluyó la revisión detallada de la configuración de sesiones, identificando que no se había configurado un timeout adecuado, permitiendo que las sesiones permanecieran abiertas indefinidamente. También analicé los mecanismos de control de acceso, documentando que los permisos de módulos solo se validaban en el cliente sin verificación en el servidor.

Además, evalué el procesamiento de XML en la aplicación, documentando la falta de protección contra ataques XXE. También analicé las transacciones financieras, identificando que no se implementaban operaciones atómicas, lo cual permitía condiciones de carrera y posibles errores de lógica de negocio. Colaboré con el equipo en la validación de los hallazgos y en la redacción de remediaciones técnicas específicas para cada vulnerabilidad.

---

## Conclusión

El trabajo realizado en este proyecto ha sido fundamental para comprender la importancia crítica del testing de seguridad y la implementación de medidas de protección adecuadas en aplicaciones web. Aunque las vulnerabilidades identificadas son de severidad baja, demuestran que incluso los aspectos aparentemente menores de una aplicación pueden representar riesgos de seguridad que deben ser abordados.

La seguridad web requiere atención a todos los detalles, desde el manejo de errores hasta la lógica de negocio y la gestión de sesiones. El testing de seguridad sistemático es esencial para identificar vulnerabilidades en todos los niveles, incluso aquellas que pueden parecer menores pero que pueden ser explotadas en combinación con otras vulnerabilidades. Este proyecto ha reforzado mi comprensión de que la seguridad es un aspecto integral que debe considerarse en cada detalle del desarrollo, y que no hay vulnerabilidades demasiado pequeñas para ser ignoradas.

---

**Preparado por:** Carlos  
**Fecha:** 2024-12-19



