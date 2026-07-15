# AWS Certified Cloud Practitioner (CLF-C02)
# Dominio 3 - Tecnología y Servicios de la Nube (34%)

**Navegación:** [Inicio](../README.md) · [Anterior: Preguntas - Dominio 2](../CLF-C02-Questions/CLF-C02-Questions-D2.md) · [Siguiente: Preguntas - Dominio 3](../CLF-C02-Questions/CLF-C02-Questions-D3.md)

---

# Semana 5 - Tareas 3.1 y 3.2 Despliegue, operación e infraestructura global

## Objetivos
-   Definir métodos para desplegar y operar en AWS.
-   Describir Regiones, zonas de disponibilidad y ubicaciones de borde.

## - Módulo 1 - Métodos de despliegue y operación (Tarea 3.1)

### Temas
-   AWS Management Console
-   AWS CLI
-   AWS SDK y APIs (acceso programático)
-   Infraestructura como código: AWS CloudFormation
-   AWS Elastic Beanstalk
-   Operaciones únicas vs. procesos repetibles
-   Modelos de despliegue: nube, híbrido y on-premises
-   AWS Outposts y AWS Systems Manager

### Laboratorio
-   Crear un bucket S3 desde la consola, la CLI y una plantilla de CloudFormation.
-   Comparar la repetibilidad de cada método.

### Documentación oficial
-   [AWS CLI](https://docs.aws.amazon.com/cli/)
-   [AWS CloudFormation](https://docs.aws.amazon.com/cloudformation/)
-   [AWS Elastic Beanstalk](https://docs.aws.amazon.com/elasticbeanstalk/)
-   [Herramientas para AWS](https://aws.amazon.com/developer/tools/)

------------------------------------------------------------------------

## - Módulo 2 - Infraestructura global (Tarea 3.2)

### Temas
-   Regiones de AWS
-   Zonas de disponibilidad (AZ): no comparten puntos únicos de fallo
-   Ubicaciones de borde (edge locations) y Amazon CloudFront
-   Alta disponibilidad con múltiples AZ
-   Uso de múltiples Regiones: recuperación ante desastres, continuidad del negocio, baja latencia y soberanía de datos
-   Criterios para elegir una Región (cumplimiento, latencia, precio, disponibilidad de servicios)
-   AWS Local Zones y AWS Wavelength (conceptos)

### Laboratorio
-   Revisar el mapa de infraestructura global de AWS.
-   Lanzar recursos en dos AZ distintas dentro de una Región.

### Documentación oficial
-   [Infraestructura global de AWS](https://aws.amazon.com/about-aws/global-infrastructure/)
-   [Regiones y zonas de disponibilidad](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/)

------------------------------------------------------------------------

# Semana 6 - Tareas 3.3 a 3.5 Cómputo, bases de datos y redes

## Objetivos
-   Identificar servicios de cómputo, bases de datos y redes.

## - Módulo 3 - Servicios de cómputo (Tarea 3.3)

### Temas
-   Amazon EC2 y familias de instancias (propósito general, optimizadas para cómputo, memoria, almacenamiento y computación acelerada)
-   Contenedores: Amazon ECS, Amazon EKS y Amazon ECR
-   Serverless: AWS Lambda y AWS Fargate
-   Amazon EC2 Auto Scaling (elasticidad)
-   Elastic Load Balancing (ALB, NLB, GWLB)
-   AWS Elastic Beanstalk, Amazon Lightsail y AWS Batch
-   AWS Outposts

### Laboratorio
-   Crear un Auto Scaling group detrás de un Application Load Balancer.
-   Crear una función Lambda disparada por un evento de S3.

### Documentación oficial
-   [Amazon EC2](https://docs.aws.amazon.com/ec2/)
-   [Tipos de instancia EC2](https://aws.amazon.com/ec2/instance-types/)
-   [AWS Lambda](https://docs.aws.amazon.com/lambda/)
-   [Elastic Load Balancing](https://docs.aws.amazon.com/elasticloadbalancing/)
-   [Amazon ECS](https://docs.aws.amazon.com/ecs/)
-   [Amazon EKS](https://docs.aws.amazon.com/eks/)

------------------------------------------------------------------------

## - Módulo 4 - Servicios de bases de datos (Tarea 3.4)

### Temas
-   Base de datos en EC2 vs. bases de datos administradas
-   Relacionales: Amazon RDS y Amazon Aurora
-   NoSQL: Amazon DynamoDB y Amazon DocumentDB
-   En memoria: Amazon ElastiCache
-   Grafos: Amazon Neptune
-   Data warehouse: Amazon Redshift
-   Migración: AWS DMS y AWS SCT

### Laboratorio
-   Crear una instancia Amazon RDS Multi-AZ.
-   Crear una tabla de DynamoDB e insertar elementos.

### Documentación oficial
-   [Amazon RDS](https://docs.aws.amazon.com/rds/)
-   [Amazon Aurora](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/)
-   [Amazon DynamoDB](https://docs.aws.amazon.com/dynamodb/)
-   [Amazon ElastiCache](https://docs.aws.amazon.com/elasticache/)
-   [Bases de datos en AWS](https://aws.amazon.com/products/databases/)

------------------------------------------------------------------------

## - Módulo 5 - Servicios de red (Tarea 3.5)

### Temas
-   Amazon VPC: subredes, tablas de rutas, Internet Gateway y NAT Gateway
-   Seguridad en la VPC: grupos de seguridad (con estado) y Network ACL (sin estado)
-   Amazon Route 53 (DNS y políticas de enrutamiento)
-   Conectividad: AWS Site-to-Site VPN, AWS Client VPN y AWS Direct Connect
-   AWS Transit Gateway, VPC Peering y AWS PrivateLink
-   Amazon CloudFront y AWS Global Accelerator
-   Amazon API Gateway

### Laboratorio
-   Crear una VPC con subredes públicas y privadas.
-   Configurar un registro de Route 53 hacia un balanceador.

### Documentación oficial
-   [Amazon VPC](https://docs.aws.amazon.com/vpc/)
-   [Amazon Route 53](https://docs.aws.amazon.com/route53/)
-   [AWS Direct Connect](https://docs.aws.amazon.com/directconnect/)
-   [AWS Site-to-Site VPN](https://docs.aws.amazon.com/vpn/latest/s2svpn/)
-   [Amazon CloudFront](https://docs.aws.amazon.com/cloudfront/)

------------------------------------------------------------------------

# Semana 7 - Tareas 3.6 a 3.8 Almacenamiento, IA/ML, analítica y otros servicios

## Objetivos
-   Identificar servicios de almacenamiento, IA/ML y analítica.
-   Reconocer servicios de otras categorías incluidas en el examen.

## - Módulo 6 - Servicios de almacenamiento (Tarea 3.6)

### Temas
-   Almacenamiento de objetos: Amazon S3
-   Clases de almacenamiento de S3 (Standard, Intelligent-Tiering, Standard-IA, One Zone-IA, Glacier Instant/Flexible/Deep Archive)
-   Almacenamiento en bloque: Amazon EBS e instance store
-   Sistemas de archivos: Amazon EFS y Amazon FSx
-   Almacenamiento híbrido con caché: AWS Storage Gateway
-   Políticas de ciclo de vida
-   AWS Backup y AWS Elastic Disaster Recovery

### Laboratorio
-   Crear un bucket S3 con una regla de ciclo de vida.
-   Adjuntar un volumen EBS a una instancia EC2.
-   Crear un plan de AWS Backup.

### Documentación oficial
-   [Amazon S3](https://docs.aws.amazon.com/s3/)
-   [Clases de almacenamiento de S3](https://aws.amazon.com/s3/storage-classes/)
-   [Amazon EBS](https://docs.aws.amazon.com/ebs/)
-   [Amazon EFS](https://docs.aws.amazon.com/efs/)
-   [AWS Backup](https://docs.aws.amazon.com/aws-backup/)

------------------------------------------------------------------------

## - Módulo 7 - IA/ML y analítica (Tarea 3.7)

### Temas
-   Amazon SageMaker AI (construcción de modelos)
-   Amazon Lex (chatbots), Amazon Polly (texto a voz), Amazon Transcribe (voz a texto) y Amazon Translate
-   Amazon Rekognition (imágenes y video), Amazon Textract (documentos) y Amazon Comprehend (NLP)
-   Amazon Q (asistente generativo)
-   Amazon Athena (SQL sobre S3)
-   Amazon Kinesis (streaming)
-   AWS Glue (ETL y catálogo)
-   Amazon Quick (BI)
-   Amazon Redshift, Amazon EMR y Amazon OpenSearch Service

### Laboratorio
-   Analizar una imagen con Amazon Rekognition.
-   Consultar un archivo CSV en S3 con Amazon Athena.

### Documentación oficial
-   [Amazon SageMaker AI](https://docs.aws.amazon.com/sagemaker/)
-   [Amazon Rekognition](https://docs.aws.amazon.com/rekognition/)
-   [Amazon Athena](https://docs.aws.amazon.com/athena/)
-   [AWS Glue](https://docs.aws.amazon.com/glue/)
-   [Amazon Kinesis](https://docs.aws.amazon.com/kinesis/)

------------------------------------------------------------------------

## - Módulo 8 - Otras categorías de servicios (Tarea 3.8)

### Temas
-   Integración de aplicaciones: Amazon SNS, Amazon SQS, Amazon EventBridge y AWS Step Functions
-   Aplicaciones empresariales: Amazon Connect y Amazon SES
-   Habilitación del cliente: AWS Support
-   Herramientas para desarrolladores: AWS CodeBuild, AWS CodePipeline y AWS X-Ray
-   Computación para el usuario final: Amazon WorkSpaces, Amazon AppStream 2.0 y WorkSpaces Secure Browser
-   Frontend web y móvil: AWS Amplify
-   IoT: AWS IoT Core

### Laboratorio
-   Crear un tema SNS con una suscripción de correo.
-   Crear una cola SQS y enviar un mensaje.

### Documentación oficial
-   [Amazon SNS](https://docs.aws.amazon.com/sns/)
-   [Amazon SQS](https://docs.aws.amazon.com/sqs/)
-   [Amazon EventBridge](https://docs.aws.amazon.com/eventbridge/)
-   [AWS CodePipeline](https://docs.aws.amazon.com/codepipeline/)
-   [Amazon WorkSpaces](https://docs.aws.amazon.com/workspaces/)
-   [AWS IoT Core](https://docs.aws.amazon.com/iot/)

------------------------------------------------------------------------

# Servicios y conceptos del dominio
-   Amazon EC2, Auto Scaling, ELB, Lambda, Fargate, ECS, EKS y ECR
-   Amazon RDS, Aurora, DynamoDB, ElastiCache, Neptune y DocumentDB
-   Amazon VPC, Route 53, CloudFront, Direct Connect, VPN y Transit Gateway
-   Amazon S3, EBS, EFS, FSx, Storage Gateway y AWS Backup
-   SageMaker AI, Lex, Polly, Rekognition, Transcribe, Translate, Textract y Comprehend
-   Athena, Kinesis, Glue y Quick
-   SNS, SQS y EventBridge
-   Amazon Connect, SES, WorkSpaces, AppStream 2.0, Amplify e IoT Core

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
-   [Productos de AWS](https://aws.amazon.com/products/)
-   [AWS Documentation](https://docs.aws.amazon.com/)
-   [AWS Skill Builder](https://explore.skillbuilder.aws/)
-   [Guía oficial del examen CLF-C02](https://docs.aws.amazon.com/aws-certification/latest/cloud-practitioner-02/cloud-practitioner-02.html)

------------------------------------------------------------------------

# Objetivo
Al finalizar este dominio podrás posicionar los servicios centrales de AWS (cómputo, bases de datos, redes, almacenamiento, IA/ML y analítica) e identificar el servicio adecuado para casos de uso comunes.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Preguntas - Dominio 2](../CLF-C02-Questions/CLF-C02-Questions-D2.md) · [Siguiente: Preguntas - Dominio 3](../CLF-C02-Questions/CLF-C02-Questions-D3.md)
