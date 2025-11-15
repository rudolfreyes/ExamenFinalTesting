# Reporte de Vulnerabilidades — Manuel

**Fecha:** 2024-12-19  
**Proyecto:** Vulnerable Accounting System  
**Grupo de Testing**

---

## Resumen

Durante el análisis de seguridad del sistema Vulnerable Accounting System, identifiqué y documenté **5 vulnerabilidades críticas** que representan riesgos significativos para la seguridad del sistema. Estas vulnerabilidades se encuentran en los rangos 6 a 10 y abarcan problemas relacionados con la exposición de credenciales, bypass de autenticación, ejecución de código SQL sin validación, eliminación masiva de datos y exposición de claves de aplicación.

---

## Vulnerabilidades Identificadas

### Vulnerabilidad 6: Exposición masiva de credenciales y secretos
**Severidad:** Critical

### Vulnerabilidad 7: Admin Bypass Token Hardcodeado
**Severidad:** Critical

### Vulnerabilidad 8: Ejecución SQL directa sin validación
**Severidad:** Critical

### Vulnerabilidad 9: Eliminación masiva de datos sin confirmación
**Severidad:** Critical

### Vulnerabilidad 10: Exposición de App Key de Laravel
**Severidad:** Critical

---

## Mi Contribución al Proyecto

Durante el desarrollo de este proyecto de análisis de seguridad, me enfoqué en la identificación y documentación de vulnerabilidades críticas relacionadas con la exposición de información sensible y el control de acceso. Realicé un análisis exhaustivo del código fuente, específicamente en los controladores de Debug, Admin y Auth, donde identifiqué múltiples endpoints que exponían credenciales de base de datos, contraseñas y variables de entorno completas.

Mi trabajo incluyó la revisión detallada de los archivos de configuración, rutas de la API y controladores para identificar puntos donde se exponía información sensible. Documenté cada vulnerabilidad con evidencia específica, incluyendo números de línea y ejemplos de código. Además, colaboré estrechamente con el equipo para validar los hallazgos y asegurar que las vulnerabilidades fueran correctamente categorizadas según su severidad e impacto.

También participé en la redacción de las remediaciones para cada vulnerabilidad identificada, proporcionando recomendaciones técnicas específicas basadas en las mejores prácticas de seguridad y estándares OWASP. Mi análisis contribuyó significativamente a identificar que el sistema presentaba fallos fundamentales en la protección de datos sensibles y en los mecanismos de autenticación y autorización.

---

## Conclusión

El trabajo realizado en este proyecto ha sido fundamental para comprender la importancia crítica del testing de seguridad y la implementación de medidas de protección adecuadas en aplicaciones web. Las vulnerabilidades identificadas demuestran que incluso sistemas aparentemente funcionales pueden contener fallos de seguridad graves que comprometen completamente la integridad, confidencialidad y disponibilidad de los datos.

La seguridad web no es un aspecto que pueda ser tratado como una consideración secundaria, sino que debe integrarse desde las primeras etapas del desarrollo. El testing de seguridad sistemático y continuo es esencial para identificar y remediar vulnerabilidades antes de que sean explotadas por atacantes. Este proyecto ha reforzado mi comprensión de que la seguridad es una responsabilidad compartida que requiere atención constante y actualización de conocimientos sobre las últimas amenazas y técnicas de mitigación.

---

**Preparado por:** Manuel  
**Fecha:** 2024-12-19



