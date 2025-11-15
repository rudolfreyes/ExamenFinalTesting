# Reporte de Vulnerabilidades — Oscar

**Proyecto:** Vulnerable Accounting System  
**Grupo de Testing**

---

## Resumen

Durante el análisis de seguridad del sistema Vulnerable Accounting System, identifiqué y documenté **5 vulnerabilidades críticas** que representan riesgos significativos para la seguridad del sistema. Estas vulnerabilidades se encuentran en los rangos 11 a 15 y abarcan problemas relacionados con la exposición de variables de entorno, path traversal, inyección de comandos, control de acceso y vulnerabilidades de scripting cruzado.

---

## Vulnerabilidades Identificadas

### Vulnerabilidad 11: Exposición de variables de entorno completas
**Severidad:** Critical

### Vulnerabilidad 12: Path Traversal en lectura de archivos
**Severidad:** Critical

### Vulnerabilidad 13: Inyección de comandos en backup
**Severidad:** Critical

### Vulnerabilidad 14: IDOR (Insecure Direct Object References)
**Severidad:** High

### Vulnerabilidad 15: Cross-Site Scripting (XSS) Reflejado y Almacenado
**Severidad:** High

---

## Mi Contribución al Proyecto

Durante el desarrollo de este proyecto de análisis de seguridad, me enfoqué en la identificación y documentación de vulnerabilidades críticas relacionadas con la exposición de información del sistema, el control de acceso y las vulnerabilidades de inyección. Realicé un análisis exhaustivo de los endpoints de debug y administración, identificando múltiples vectores de ataque que permitían acceso no autorizado a información sensible del sistema.

Mi trabajo incluyó la revisión detallada de las rutas web y los controladores para identificar endpoints que exponían variables de entorno completas, así como la evaluación de funcionalidades de lectura de archivos que eran vulnerables a path traversal. Documenté cada vulnerabilidad con evidencia específica, incluyendo ejemplos de payloads de explotación y el impacto potencial de cada una.

También analicé los mecanismos de control de acceso, identificando vulnerabilidades IDOR que permitían a usuarios acceder a recursos de otros usuarios mediante la manipulación de parámetros. Además, evalué las funcionalidades de la aplicación para identificar vulnerabilidades de Cross-Site Scripting tanto reflejadas como almacenadas. Colaboré con el equipo en la validación de los hallazgos y en la redacción de remediaciones técnicas específicas para cada vulnerabilidad.

---

## Conclusión

El trabajo realizado en este proyecto ha sido fundamental para comprender la importancia crítica del testing de seguridad y la implementación de medidas de protección adecuadas en aplicaciones web. Las vulnerabilidades identificadas demuestran que los sistemas deben implementar controles de acceso robustos, validación estricta de entradas y sanitización de salidas para prevenir ataques comunes.

La seguridad web requiere un enfoque integral que considere no solo la funcionalidad de la aplicación, sino también los mecanismos de protección que previenen el acceso no autorizado y la exposición de información sensible. El testing de seguridad sistemático es esencial para identificar vulnerabilidades antes de que sean explotadas. Este proyecto ha reforzado mi comprensión de que la seguridad es un proceso continuo que requiere atención constante y actualización de conocimientos sobre las últimas amenazas y técnicas de mitigación.

---

**Preparado por:** Oscar  