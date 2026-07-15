# Responsabilidad compartida y seguridad (CLF-C02)

**Dominio relacionado:** Dominio 2 - Seguridad y Cumplimiento (30 %)

---

## 1. Modelo de responsabilidad compartida

| AWS: seguridad **de** la nube | Cliente: seguridad **en** la nube |
|---|---|
| Hardware e instalaciones físicas | Datos y su clasificación |
| Red global y regiones | Configuración de IAM |
| Software de virtualización | Grupos de seguridad y firewalls |
| Servicios administrados (infraestructura) | Cifrado de datos |
| | Parches del sistema operativo en EC2 |

### Cómo cambia según el servicio

| Servicio | AWS administra | El cliente administra |
|---|---|---|
| Amazon EC2 | Hardware y virtualización | Sistema operativo, parches, aplicaciones, datos y red |
| Amazon RDS | Hardware, SO y parches del motor | Datos, usuarios, reglas de red y parámetros |
| AWS Lambda | Servidores, SO y entorno de ejecución | Código, permisos y datos |
| Amazon S3 | Infraestructura | Permisos del bucket, cifrado y clasificación de datos |

Tipos de controles: **heredados** (el cliente los hereda de AWS), **compartidos** (aplican a ambos, como la gestión de parches o la concienciación) y **específicos del cliente**.

---

## 2. IAM

| Elemento | Descripción |
|---|---|
| Usuario | Identidad con credenciales permanentes |
| Grupo | Conjunto de usuarios que comparten permisos |
| Rol | Identidad con credenciales temporales, asumida por usuarios, servicios o cuentas |
| Política | Documento JSON que define permisos |

- **Mínimo privilegio:** conceder solo los permisos necesarios.
- **Usuario root:** protegerlo con MFA, no crear access keys, usarlo solo para tareas que lo requieren (por ejemplo, cambiar el plan de soporte o cerrar la cuenta).
- **Roles:** para aplicaciones en EC2 y accesos entre cuentas.
- **IAM Identity Center:** SSO para varias cuentas.
- **Secrets Manager:** almacena y rota credenciales y secretos.
- **Federación:** usar identidades externas (por ejemplo, Active Directory).

---

## 3. Servicios de seguridad: ¿cuál elijo?

| Necesidad | Servicio |
|---|---|
| Descargar informes de cumplimiento | AWS Artifact |
| Auditar llamadas a la API | AWS CloudTrail |
| Historial y cumplimiento de configuraciones | AWS Config |
| Métricas y alarmas | Amazon CloudWatch |
| Detectar amenazas | Amazon GuardDuty |
| Escanear vulnerabilidades en EC2, ECR y Lambda | Amazon Inspector |
| Descubrir datos sensibles en S3 | Amazon Macie |
| Visión centralizada de seguridad | AWS Security Hub |
| Investigar la causa de un hallazgo | Amazon Detective |
| Proteger contra DDoS | AWS Shield |
| Filtrar tráfico web (SQLi, XSS) | AWS WAF |
| Administrar reglas de firewall de varias cuentas | AWS Firewall Manager |
| Administrar claves de cifrado | AWS KMS |
| HSM dedicado | AWS CloudHSM |
| Certificados TLS | AWS Certificate Manager |
| Identidad para usuarios de apps web/móviles | Amazon Cognito |
| Active Directory administrado | AWS Directory Service |
| Compartir recursos entre cuentas | AWS RAM |

---

## 4. Cifrado

- **En tránsito:** protege los datos que viajan por la red (TLS/HTTPS).
- **En reposo:** protege los datos almacenados (S3, EBS, RDS con KMS).

---

## 5. Seguridad de red

| Característica | Security group | Network ACL |
|---|---|---|
| Nivel | Instancia (ENI) | Subred |
| Estado | Con estado | Sin estado |
| Reglas | Solo permitir | Permitir y denegar |

---

## 6. Dónde encontrar información de seguridad

- AWS Knowledge Center
- AWS Security Center
- AWS Security Blog
- AWS Trusted Advisor (categoría de seguridad)
- AWS Marketplace (productos de seguridad de terceros)

---

## Checklist final

- [ ] Clasificar una tarea como responsabilidad de AWS o del cliente para EC2, RDS y Lambda.
- [ ] Listar las tareas que solo puede hacer el usuario root.
- [ ] Elegir el servicio de seguridad correcto a partir de un requisito.
- [ ] Diferenciar security group y Network ACL.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Valor de la nube](01-Cloud-Value-and-Well-Architected.md) · [Siguiente: Comparativa de servicios](03-Core-Services-Comparison.md)
