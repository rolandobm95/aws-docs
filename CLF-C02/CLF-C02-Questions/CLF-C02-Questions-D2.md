# Preguntas de Práctica - Dominio 2: Seguridad y Cumplimiento

**Navegación:** [Inicio](../README.md) · [Anterior: Dominio 2](../CLF-C02-Domains/CLF-C02-Domain-2.md) · [Siguiente: Dominio 3](../CLF-C02-Domains/CLF-C02-Domain-3.md)

---

## Tarea 2.1 - Entender el modelo de responsabilidad compartida de AWS

### Pregunta 1
Según el modelo de responsabilidad compartida, ¿cuál de las siguientes tareas es responsabilidad de AWS?
- A) Aplicar parches al sistema operativo de las instancias EC2.
- B) Administrar el hardware y las instalaciones físicas de los centros de datos.
- C) Configurar los grupos de seguridad de las instancias.
- D) Cifrar los datos del cliente en reposo en cada aplicación.

---

### Pregunta 2
Una empresa ejecuta su base de datos en Amazon RDS. ¿Qué tarea de parches sigue siendo responsabilidad de AWS en este caso?
- A) Parchear el sistema operativo y el motor de base de datos subyacentes.
- B) Definir los usuarios y permisos de la base de datos.
- C) Decidir qué datos se almacenan.
- D) Configurar las reglas del grupo de seguridad.

---

### Pregunta 3
¿Cuáles de las siguientes son responsabilidades **del cliente** en AWS? (Seleccione DOS)
- A) Proteger los datos que almacena en Amazon S3.
- B) Mantener el equipamiento físico del centro de datos.
- C) Administrar los permisos de IAM.
- D) Operar la red global de AWS.
- E) Controlar el acceso físico a los edificios de AWS.

---

## Tarea 2.2 - Entender los conceptos de seguridad, gobernanza y cumplimiento de la nube de AWS

### Pregunta 4
Un auditor solicita los informes de cumplimiento SOC e ISO de AWS. ¿Dónde puede descargarlos la empresa?
- A) AWS Config
- B) Amazon Inspector
- C) AWS Artifact
- D) AWS Trusted Advisor

---

### Pregunta 5
Una empresa necesita saber quién eliminó un grupo de seguridad y cuándo. ¿Qué servicio debe consultar?
- A) AWS Shield
- B) Amazon CloudWatch
- C) AWS CloudTrail
- D) Amazon Macie

---

## Tarea 2.3 - Identificar las capacidades de administración de acceso de AWS

### Pregunta 6
¿Cuál es la mejor práctica para proteger el usuario root de una cuenta de AWS?
- A) Crear access keys para el root y usarlas en scripts.
- B) Habilitar MFA y evitar su uso para tareas cotidianas.
- C) Eliminar el usuario root.
- D) Compartir sus credenciales con el equipo de administración.

---

### Pregunta 7
Una aplicación en EC2 necesita leer objetos de S3 sin guardar credenciales de larga duración en el código. ¿Qué debe usar?
- A) Una contraseña almacenada en una variable de entorno.
- B) Un usuario IAM con access keys en un archivo de configuración.
- C) Las credenciales del usuario root.
- D) Un rol de IAM asociado a la instancia.

---

### Pregunta 8
Una empresa con muchas cuentas de AWS quiere que sus empleados inicien sesión una sola vez con sus credenciales corporativas y accedan a las cuentas asignadas. ¿Qué servicio ofrece esta capacidad?
- A) AWS KMS
- B) AWS IAM Identity Center
- C) Amazon Inspector
- D) AWS WAF

---

## Tarea 2.4 - Identificar componentes y recursos de seguridad

### Pregunta 9
¿Qué servicio analiza continuamente los registros de CloudTrail, VPC Flow Logs y DNS para detectar actividad maliciosa o no autorizada?
- A) Amazon Cognito
- B) AWS Shield
- C) AWS Artifact
- D) Amazon GuardDuty

---

### Pregunta 10
Una empresa quiere protegerse contra ataques web comunes como inyección SQL y cross-site scripting en su aplicación detrás de Application Load Balancer. ¿Qué servicio debe usar?
- A) AWS Config
- B) AWS CloudTrail
- C) AWS WAF
- D) Amazon Macie

---

# Respuestas y Explicaciones

### Pregunta 1
**Respuesta correcta: B**
**Explicación:** AWS es responsable de la seguridad **de** la nube: hardware, software base, red e instalaciones físicas. El cliente es responsable de la seguridad **en** la nube: datos, configuración de grupos de seguridad y parches del sistema operativo en EC2.

### Pregunta 2
**Respuesta correcta: A**
**Explicación:** En un servicio administrado como RDS, AWS parchea el sistema operativo y gestiona la infraestructura del motor. El cliente conserva la gestión de usuarios, datos y reglas de red.

### Pregunta 3
**Respuesta correcta: A, C**
**Explicación:** El cliente es responsable de sus datos y de la administración de identidades y permisos. El hardware, la red global y la seguridad física son responsabilidad de AWS.

### Pregunta 4
**Respuesta correcta: C**
**Explicación:** AWS Artifact es el portal de autoservicio para descargar informes de cumplimiento y aceptar acuerdos. Config registra configuraciones, Inspector escanea vulnerabilidades y Trusted Advisor ofrece recomendaciones.

### Pregunta 5
**Respuesta correcta: C**
**Explicación:** CloudTrail registra las llamadas a la API (quién, qué, cuándo y desde dónde). CloudWatch monitorea métricas y logs, Shield protege contra DDoS y Macie detecta datos sensibles en S3.

### Pregunta 6
**Respuesta correcta: B**
**Explicación:** Se debe proteger el root con MFA y usarlo solo para las tareas que lo requieren. No se puede eliminar el usuario root y no se recomienda crear access keys para él.

### Pregunta 7
**Respuesta correcta: D**
**Explicación:** Los roles de IAM entregan credenciales temporales a la instancia y evitan almacenar claves de larga duración. Las demás opciones son prácticas inseguras.

### Pregunta 8
**Respuesta correcta: B**
**Explicación:** IAM Identity Center ofrece inicio de sesión único (SSO) centralizado para varias cuentas y aplicaciones. KMS administra claves, WAF filtra tráfico web e Inspector busca vulnerabilidades.

### Pregunta 9
**Respuesta correcta: D**
**Explicación:** GuardDuty es un servicio de detección de amenazas que analiza múltiples fuentes de datos. Shield protege contra DDoS, Cognito gestiona identidades de aplicaciones y Artifact entrega informes de cumplimiento.

### Pregunta 10
**Respuesta correcta: C**
**Explicación:** AWS WAF es un firewall de aplicaciones web que filtra solicitudes HTTP/HTTPS con reglas que bloquean patrones como SQL injection o XSS. Los demás servicios no filtran tráfico de aplicaciones.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Dominio 2](../CLF-C02-Domains/CLF-C02-Domain-2.md) · [Siguiente: Dominio 3](../CLF-C02-Domains/CLF-C02-Domain-3.md)
