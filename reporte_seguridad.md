# Reporte de Vulnerabilidades — Keisy

**Fecha:** 2024-12-19  
**Proyecto:** Vulnerable Accounting System  
**Grupo de Testing**

---

## Resumen

Durante el análisis de seguridad del sistema Vulnerable Accounting System, identifiqué y documenté **5 vulnerabilidades de alta severidad** que representan riesgos significativos para la seguridad del sistema. Estas vulnerabilidades se encuentran en los rangos 16 a 20 y abarcan problemas relacionados con la configuración de CORS, subida de archivos sin validación, gestión de sesiones, modo debug en producción y credenciales débiles por defecto.

---

## Vulnerabilidades Identificadas

### Vulnerabilidad 16: CORS extremadamente permisivo
**Severidad:** High

### Vulnerabilidad 17: Subida de archivos sin validación
**Severidad:** High

### Vulnerabilidad 18: Gestión insegura de sesiones
**Severidad:** High

### Vulnerabilidad 19: Debug mode habilitado en producción
**Severidad:** High

### Vulnerabilidad 20: Credenciales débiles por defecto
**Severidad:** High

---

## Mi Contribución al Proyecto

Durante el desarrollo de este proyecto de análisis de seguridad, me enfoqué en la identificación y documentación de vulnerabilidades relacionadas con la configuración de seguridad, la gestión de sesiones y las políticas de autenticación. Realicé un análisis exhaustivo de los archivos de configuración, específicamente en la configuración de CORS, donde identifiqué que el sistema permitía solicitudes desde cualquier origen con credenciales habilitadas.

Mi trabajo incluyó la revisión detallada de los mecanismos de autenticación y gestión de sesiones, identificando que las sesiones almacenaban información sensible como contraseñas y que los tokens de sesión eran predecibles. También analicé las funcionalidades de subida de archivos, documentando la falta de validación de tipo, tamaño y contenido de los archivos subidos.

Además, evalué la configuración del entorno de producción, identificando que el modo debug estaba habilitado y que el sistema incluía credenciales por defecto débiles y predecibles. Documenté cada vulnerabilidad con evidencia específica, incluyendo ubicaciones en el código y ejemplos de configuración problemática. Colaboré con el equipo en la validación de los hallazgos y en la redacción de remediaciones técnicas específicas para cada vulnerabilidad.

---

## Conclusión

El trabajo realizado en este proyecto ha sido fundamental para comprender la importancia crítica del testing de seguridad y la implementación de medidas de protección adecuadas en aplicaciones web. Las vulnerabilidades identificadas demuestran que la configuración de seguridad es tan importante como la implementación de funcionalidades, y que pequeños descuidos en la configuración pueden resultar en vulnerabilidades significativas.

La seguridad web requiere atención a los detalles en todos los aspectos del sistema, desde la configuración de CORS hasta la gestión de sesiones y las políticas de autenticación. El testing de seguridad sistemático es esencial para identificar configuraciones inseguras y vulnerabilidades antes de que sean explotadas. Este proyecto ha reforzado mi comprensión de que la seguridad es un aspecto integral que debe considerarse en cada etapa del desarrollo y despliegue de aplicaciones web.

---

**Preparado por:** Keisy  
**Fecha:** 2024-12-19



