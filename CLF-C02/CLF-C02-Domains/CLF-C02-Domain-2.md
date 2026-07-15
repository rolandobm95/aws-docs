# AWS Certified Cloud Practitioner (CLF-C02)
# Dominio 2 - Seguridad y Cumplimiento (30%)

**Navegación:** [Inicio](../README.md) · [Anterior: Preguntas - Dominio 1](../CLF-C02-Questions/CLF-C02-Questions-D1.md) · [Siguiente: Preguntas - Dominio 2](../CLF-C02-Questions/CLF-C02-Questions-D2.md)

---

# Semana 3 - Tareas 2.1 y 2.2 Responsabilidad compartida, gobernanza y cumplimiento

## Objetivos
-   Entender el modelo de responsabilidad compartida.
-   Reconocer conceptos de seguridad, gobernanza y cumplimiento.
-   Identificar dónde encontrar información de cumplimiento y logs.

## - Módulo 1 - Modelo de responsabilidad compartida (Tarea 2.1)

### Temas
-   Responsabilidad de AWS: seguridad **de** la nube (hardware, software, red e instalaciones)
-   Responsabilidad del cliente: seguridad **en** la nube (datos, IAM, configuración, cifrado)
-   Controles heredados, compartidos y específicos del cliente
-   Cómo cambia la responsabilidad según el servicio: Amazon EC2 (IaaS), Amazon RDS (administrado) y AWS Lambda (serverless)
-   Parches del sistema operativo, del motor de base de datos y de la aplicación

### Laboratorio
-   Dibujar una tabla de responsabilidades para EC2, RDS y Lambda.
-   Identificar quién parchea el sistema operativo en cada caso.

### Documentación oficial
-   [Modelo de responsabilidad compartida](https://aws.amazon.com/compliance/shared-responsibility-model/)
-   [Security Pillar - Well-Architected](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/welcome.html)

------------------------------------------------------------------------

## - Módulo 2 - Seguridad, gobernanza y cumplimiento (Tarea 2.2)

### Temas
-   AWS Artifact (informes de cumplimiento y acuerdos)
-   Programas de cumplimiento (ISO, SOC, PCI DSS, GDPR, HIPAA)
-   Requisitos de cumplimiento por región o industria
-   Cifrado en tránsito y en reposo
-   AWS KMS y AWS CloudHSM
-   AWS Certificate Manager (ACM)
-   Amazon CloudWatch (monitoreo)
-   AWS CloudTrail (auditoría de llamadas a la API)
-   AWS Config (historial y cumplimiento de configuraciones)
-   Reportes de acceso (IAM credential report, IAM Access Analyzer)
-   AWS Audit Manager

### Laboratorio
-   Descargar un informe en AWS Artifact.
-   Habilitar un trail de CloudTrail y localizar un evento.
-   Activar una regla administrada de AWS Config.

### Documentación oficial
-   [AWS Artifact](https://docs.aws.amazon.com/artifact/)
-   [AWS CloudTrail](https://docs.aws.amazon.com/awscloudtrail/)
-   [AWS Config](https://docs.aws.amazon.com/config/)
-   [AWS KMS](https://docs.aws.amazon.com/kms/)
-   [Programas de cumplimiento de AWS](https://aws.amazon.com/compliance/programs/)

------------------------------------------------------------------------

# Semana 4 - Tareas 2.3 y 2.4 Gestión de acceso y recursos de seguridad

## Objetivos
-   Identificar capacidades de administración de acceso.
-   Reconocer servicios y recursos de seguridad de AWS.

## - Módulo 3 - Administración de acceso (Tarea 2.3)

### Temas
-   AWS IAM: usuarios, grupos, roles y políticas
-   Políticas administradas por AWS vs. políticas personalizadas
-   Principio de mínimo privilegio
-   Usuario root: importancia de protegerlo y tareas que solo el root puede realizar
-   MFA y políticas de contraseñas
-   Access keys y almacenamiento de credenciales
-   AWS Secrets Manager y AWS Systems Manager Parameter Store
-   AWS IAM Identity Center (SSO)
-   Roles IAM entre cuentas
-   Identidad federada
-   Amazon Cognito y AWS Directory Service

### Laboratorio
-   Habilitar MFA en el usuario root.
-   Crear un grupo con una política de solo lectura y asignar un usuario.
-   Crear un rol IAM para EC2.

### Documentación oficial
-   [AWS IAM](https://docs.aws.amazon.com/IAM/)
-   [Prácticas recomendadas de seguridad en IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)
-   [Tareas que requieren credenciales root](https://docs.aws.amazon.com/IAM/latest/UserGuide/root-user-tasks.html)
-   [AWS IAM Identity Center](https://docs.aws.amazon.com/singlesignon/)
-   [AWS Secrets Manager](https://docs.aws.amazon.com/secretsmanager/)

------------------------------------------------------------------------

## - Módulo 4 - Componentes y recursos de seguridad (Tarea 2.4)

### Temas
-   AWS WAF (firewall de aplicaciones web)
-   AWS Shield Standard y Advanced (DDoS)
-   AWS Firewall Manager
-   Amazon GuardDuty (detección de amenazas)
-   Amazon Inspector (vulnerabilidades)
-   AWS Security Hub
-   Amazon Macie (datos sensibles en S3)
-   Amazon Detective
-   Grupos de seguridad y Network ACL
-   AWS Trusted Advisor (categoría de seguridad)
-   Productos de seguridad de terceros en AWS Marketplace
-   Recursos: AWS Knowledge Center, AWS Security Center y AWS Security Blog

### Laboratorio
-   Habilitar GuardDuty y revisar los hallazgos de ejemplo.
-   Comparar un grupo de seguridad con una Network ACL.
-   Revisar las comprobaciones de seguridad de Trusted Advisor.

### Documentación oficial
-   [Amazon GuardDuty](https://docs.aws.amazon.com/guardduty/)
-   [Amazon Inspector](https://docs.aws.amazon.com/inspector/)
-   [AWS Security Hub](https://docs.aws.amazon.com/securityhub/)
-   [AWS WAF](https://docs.aws.amazon.com/waf/)
-   [AWS Shield](https://docs.aws.amazon.com/shield/)
-   [AWS Security Blog](https://aws.amazon.com/blogs/security/)

------------------------------------------------------------------------

# Servicios y conceptos del dominio
-   AWS Artifact
-   AWS IAM e IAM Identity Center
-   AWS KMS, CloudHSM y ACM
-   AWS Secrets Manager
-   Amazon Cognito y AWS Directory Service
-   AWS WAF, AWS Shield y AWS Firewall Manager
-   Amazon GuardDuty, Amazon Inspector, Amazon Macie, Amazon Detective y AWS Security Hub
-   AWS CloudTrail, Amazon CloudWatch y AWS Config
-   AWS Trusted Advisor

---

# Notas Personales

## Conceptos Clave
<!-- Anota aquí los conceptos más importantes que debes recordar para el examen -->
-

## Áreas de Mejora
<!-- Registra los temas donde te sientes menos seguro y necesitas repasar -->
-

## Trucos para el Examen
<!-- Anota patrones de preguntas, palabras clave que identifican servicios, o atajos para resolver escenarios -->
-

------------------------------------------------------------------------

# Recursos Oficiales
-   [AWS Security](https://aws.amazon.com/security/)
-   [AWS Compliance](https://aws.amazon.com/compliance/)
-   [AWS Skill Builder](https://explore.skillbuilder.aws/)
-   [Guía oficial del examen CLF-C02](https://docs.aws.amazon.com/aws-certification/latest/cloud-practitioner-02/cloud-practitioner-02.html)

------------------------------------------------------------------------

# Objetivo
Al finalizar este dominio podrás explicar el modelo de responsabilidad compartida, seleccionar el servicio de seguridad adecuado y aplicar buenas prácticas de IAM.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Preguntas - Dominio 1](../CLF-C02-Questions/CLF-C02-Questions-D1.md) · [Siguiente: Preguntas - Dominio 2](../CLF-C02-Questions/CLF-C02-Questions-D2.md)
