# Comparativa de servicios centrales (CLF-C02)

**Dominio relacionado:** Dominio 3 - Tecnología y Servicios de la Nube (34 %)

---

## 1. Infraestructura global

| Concepto | Descripción |
|---|---|
| Región | Área geográfica con varias zonas de disponibilidad |
| Zona de disponibilidad (AZ) | Uno o más centros de datos aislados, sin puntos únicos de fallo compartidos |
| Ubicación de borde | Punto de presencia para entregar contenido con baja latencia (CloudFront, Route 53) |

**Cuándo usar varias Regiones:** recuperación ante desastres, continuidad del negocio, baja latencia para usuarios y soberanía de datos.

---

## 2. Formas de acceder a AWS

| Método | Uso |
|---|---|
| Consola de administración | Interfaz web, tareas puntuales |
| AWS CLI | Línea de comandos y scripts |
| SDK / API | Acceso programático desde aplicaciones |
| CloudFormation | Infraestructura como código, repetible |

---

## 3. Cómputo

| Necesidad | Servicio |
|---|---|
| Servidores virtuales | Amazon EC2 |
| Escalar instancias automáticamente | EC2 Auto Scaling |
| Distribuir tráfico | Elastic Load Balancing |
| Ejecutar código por eventos | AWS Lambda |
| Contenedores sin administrar servidores | AWS Fargate |
| Orquestar contenedores | Amazon ECS / Amazon EKS (Kubernetes) |
| Almacenar imágenes de contenedor | Amazon ECR |
| Desplegar apps sin administrar la infraestructura | AWS Elastic Beanstalk |
| Servidor privado virtual simple | Amazon Lightsail |
| Trabajos por lotes | AWS Batch |
| Infraestructura AWS on-premises | AWS Outposts |

### Familias de instancias EC2
| Familia | Uso |
|---|---|
| Propósito general | Cargas equilibradas |
| Optimizadas para cómputo | Procesamiento intensivo, HPC |
| Optimizadas para memoria | Bases de datos en memoria |
| Optimizadas para almacenamiento | Alto IOPS y throughput de disco |
| Computación acelerada | GPU, ML |

---

## 4. Bases de datos

| Necesidad | Servicio |
|---|---|
| Relacional administrada | Amazon RDS |
| Relacional de alto rendimiento (MySQL/PostgreSQL) | Amazon Aurora |
| NoSQL clave-valor | Amazon DynamoDB |
| Documentos compatible con MongoDB | Amazon DocumentDB |
| Caché en memoria | Amazon ElastiCache |
| Grafos | Amazon Neptune |
| Data warehouse | Amazon Redshift |
| Migrar bases | AWS DMS + AWS SCT |

**¿Base en EC2 o administrada?** Una base administrada reduce la carga operativa (parches, backups, alta disponibilidad). EC2 se elige cuando se necesita control total del sistema operativo o del motor.

---

## 5. Redes

| Necesidad | Servicio |
|---|---|
| Red virtual aislada | Amazon VPC |
| DNS | Amazon Route 53 |
| CDN | Amazon CloudFront |
| Mejorar rutas de red globales (IPs anycast) | AWS Global Accelerator |
| VPN de red a red | AWS Site-to-Site VPN |
| VPN para usuarios | AWS Client VPN |
| Conexión dedicada | AWS Direct Connect |
| Conectar muchas VPC y redes | AWS Transit Gateway |
| Acceso privado a servicios | AWS PrivateLink |
| Crear y publicar APIs | Amazon API Gateway |

---

## 6. Almacenamiento

| Tipo | Servicio |
|---|---|
| Objetos | Amazon S3 |
| Bloque | Amazon EBS (persistente), instance store (temporal) |
| Archivos Linux (NFS) | Amazon EFS |
| Archivos Windows / HPC | Amazon FSx |
| Híbrido con caché | AWS Storage Gateway |
| Respaldos | AWS Backup |
| Recuperación ante desastres | AWS Elastic Disaster Recovery |

### Clases de S3
| Clase | Uso |
|---|---|
| Standard | Acceso frecuente |
| Intelligent-Tiering | Patrones de acceso desconocidos o cambiantes |
| Standard-IA | Acceso poco frecuente, resiliencia multi-AZ |
| One Zone-IA | Acceso poco frecuente, una sola AZ |
| Glacier Instant Retrieval | Archivo con acceso en milisegundos |
| Glacier Flexible Retrieval | Archivo con recuperación en minutos u horas |
| Glacier Deep Archive | Archivo de menor costo, recuperación en horas |

Las **políticas de ciclo de vida** mueven o eliminan objetos automáticamente según su antigüedad.

---

## 7. IA/ML y analítica

| Necesidad | Servicio |
|---|---|
| Construir y entrenar modelos | Amazon SageMaker AI |
| Chatbots | Amazon Lex |
| Texto a voz | Amazon Polly |
| Voz a texto | Amazon Transcribe |
| Traducción | Amazon Translate |
| Imágenes y video | Amazon Rekognition |
| Extraer texto de documentos | Amazon Textract |
| Análisis de texto (NLP) | Amazon Comprehend |
| Asistente generativo | Amazon Q |
| SQL sobre S3 | Amazon Athena |
| Streaming | Amazon Kinesis |
| ETL y catálogo | AWS Glue |
| BI y dashboards | Amazon Quick |
| Big data (Hadoop/Spark) | Amazon EMR |
| Búsqueda y análisis de logs | Amazon OpenSearch Service |

---

## 8. Otros servicios dentro del alcance

| Necesidad | Servicio |
|---|---|
| Cola de mensajes | Amazon SQS |
| Notificaciones pub/sub | Amazon SNS |
| Bus de eventos | Amazon EventBridge |
| Flujos de trabajo | AWS Step Functions |
| Centro de contacto | Amazon Connect |
| Envío de correo | Amazon SES |
| CI/CD | AWS CodeBuild, AWS CodePipeline |
| Trazabilidad | AWS X-Ray |
| Escritorios virtuales | Amazon WorkSpaces |
| Streaming de aplicaciones | Amazon AppStream 2.0 |
| Navegador seguro | Amazon WorkSpaces Secure Browser |
| Apps web y móviles | AWS Amplify |
| Dispositivos IoT | AWS IoT Core |

---

## Checklist final

- [ ] Relacionar Región, AZ y ubicación de borde.
- [ ] Elegir el servicio de cómputo según el caso (EC2, Lambda, Fargate, ECS/EKS).
- [ ] Elegir el servicio de base de datos según el tipo de dato.
- [ ] Diferenciar VPN y Direct Connect, CloudFront y Global Accelerator.
- [ ] Diferenciar S3, EBS, EFS y FSx, y conocer las clases de S3.
- [ ] Asociar cada servicio de IA/ML con su tarea.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Responsabilidad compartida y seguridad](02-Shared-Responsibility-and-Security.md) · [Siguiente: Precios, facturación y soporte](04-Pricing-and-Support.md)
