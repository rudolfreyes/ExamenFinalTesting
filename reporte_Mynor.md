# Reporte de Vulnerabilidades — Mynor

**Fecha:** 2024-12-19  
**Proyecto:** Vulnerable Accounting System  
**Grupo de Testing**

---

## Resumen

Durante el análisis de seguridad del sistema Vulnerable Accounting System, identifiqué y documenté **5 vulnerabilidades de alta severidad** que representan riesgos significativos para la seguridad del sistema. Estas vulnerabilidades se encuentran en los rangos 21 a 25 y abarcan problemas relacionados con el reset de contraseñas, manipulación de sesiones, exposición de backups, almacenamiento inseguro de tokens y exposición de información de usuario.

---

## Vulnerabilidades Identificadas

### Vulnerabilidad 21: Reset de contraseña sin verificación
**Severidad:** High

### Vulnerabilidad 22: Manipulación de sesión sin autorización
**Severidad:** High

### Vulnerabilidad 23: Exposición de backups de base de datos
**Severidad:** High

### Vulnerabilidad 24: Almacenamiento de sesiones en localStorage
**Severidad:** High

### Vulnerabilidad 25: Exposición de información de usuario completa
**Severidad:** High

---

## Mi Contribución al Proyecto

Durante el desarrollo de este proyecto de análisis de seguridad, me enfoqué en la identificación y documentación de vulnerabilidades relacionadas con los mecanismos de autenticación, recuperación de contraseñas y gestión de sesiones. Realicé un análisis exhaustivo del controlador de autenticación, identificando que el endpoint de reset de contraseña permitía cambiar contraseñas sin verificar adecuadamente la identidad del usuario.

Mi trabajo incluyó la revisión detallada de los mecanismos de gestión de sesiones, identificando que existían endpoints que permitían la manipulación completa de sesiones sin autenticación adecuada, incluyendo la capacidad de establecer roles de administrador. También analicé las funcionalidades de backup, documentando que los backups se creaban sin encriptación y que las credenciales de base de datos se exponían en los comandos ejecutados.

Además, evalué el almacenamiento de tokens en el frontend, identificando que se utilizaba localStorage para almacenar tokens de sesión, lo cual los hacía vulnerables a ataques XSS. También documenté que los endpoints retornaban información completa de usuarios incluyendo contraseñas y API keys sin restricción. Colaboré con el equipo en la validación de los hallazgos y en la redacción de remediaciones técnicas específicas para cada vulnerabilidad.

---

## Conclusión

El trabajo realizado en este proyecto ha sido fundamental para comprender la importancia crítica del testing de seguridad y la implementación de medidas de protección adecuadas en aplicaciones web. Las vulnerabilidades identificadas demuestran que los mecanismos de autenticación y gestión de sesiones deben ser diseñados e implementados con extremo cuidado, ya que representan puntos críticos de entrada al sistema.

La seguridad web requiere una comprensión profunda de cómo funcionan los mecanismos de autenticación y autorización, y cómo pueden ser explotados por atacantes. El testing de seguridad sistemático es esencial para identificar vulnerabilidades en estos componentes críticos antes de que sean explotadas. Este proyecto ha reforzado mi comprensión de que la seguridad de la autenticación y las sesiones es fundamental para la protección general del sistema, y que pequeños descuidos pueden resultar en compromisos completos del sistema.

---

**Preparado por:** Mynor  
**Fecha:** 2024-12-19



