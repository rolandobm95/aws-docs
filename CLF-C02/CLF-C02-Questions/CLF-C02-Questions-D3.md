# Preguntas de Práctica - Dominio 3: Tecnología y Servicios de la Nube

**Navegación:** [Inicio](../README.md) · [Anterior: Dominio 3](../CLF-C02-Domains/CLF-C02-Domain-3.md) · [Siguiente: Dominio 4](../CLF-C02-Domains/CLF-C02-Domain-4.md)

---

## Tarea 3.1 - Definir métodos de despliegue y operación en la nube de AWS

### Pregunta 1
Una empresa necesita crear de forma repetible y automatizada el mismo entorno en varias cuentas. ¿Qué enfoque es el más adecuado?
- A) Crear los recursos manualmente en la consola cada vez.
- B) Usar infraestructura como código con AWS CloudFormation.
- C) Pedir a AWS Support que cree los recursos.
- D) Crear los recursos con la cuenta root.

---

## Tarea 3.2 - Definir la infraestructura global de AWS

### Pregunta 2
¿Cuál es la relación correcta entre Regiones y zonas de disponibilidad?
- A) Una Región es un único edificio.
- B) Una zona de disponibilidad contiene varias Regiones.
- C) Una Región contiene varias zonas de disponibilidad.
- D) Las zonas de disponibilidad comparten la misma fuente de energía.

---

### Pregunta 3
Una empresa quiere reducir la latencia de entrega de contenido estático a usuarios en todo el mundo. ¿Qué servicio utiliza ubicaciones de borde para lograrlo?
- A) Amazon RDS
- B) AWS Backup
- C) AWS Organizations
- D) Amazon CloudFront

---

## Tarea 3.3 - Identificar los servicios de cómputo de AWS

### Pregunta 4
Una aplicación procesa cálculos científicos que requieren muchos procesadores de alto rendimiento. ¿Qué tipo de instancia EC2 es el más adecuado?
- A) Optimizada para almacenamiento
- B) De uso general con crédito de ráfaga
- C) Optimizada para memoria
- D) Optimizada para cómputo

---

### Pregunta 5
Un equipo quiere ejecutar código en respuesta a eventos sin aprovisionar ni administrar servidores. ¿Qué servicio debe elegir?
- A) Amazon EC2
- B) Amazon Lightsail
- C) AWS Outposts
- D) AWS Lambda

---

## Tarea 3.4 - Identificar los servicios de bases de datos de AWS

### Pregunta 6
Una aplicación necesita una base de datos NoSQL clave-valor con latencia de milisegundos de un dígito y escalado automático. ¿Qué servicio es el más adecuado?
- A) Amazon DynamoDB
- B) Amazon RDS
- C) Amazon Redshift
- D) Amazon Neptune

---

### Pregunta 7
¿Qué servicio acelera aplicaciones almacenando datos consultados con frecuencia en memoria?
- A) Amazon ElastiCache
- B) Amazon Aurora
- C) Amazon DocumentDB
- D) AWS DMS

---

## Tarea 3.5 - Identificar los servicios de red de AWS

### Pregunta 8
¿Qué componente actúa como firewall virtual **con estado** a nivel de instancia en una VPC?
- A) Route table
- B) Internet gateway
- C) Network ACL
- D) Security group

---

### Pregunta 9
Una empresa necesita una conexión de red privada y dedicada entre su centro de datos y AWS que no pase por internet público. ¿Qué servicio debe usar?
- A) Amazon CloudFront
- B) AWS WAF
- C) Amazon Route 53
- D) AWS Direct Connect

---

## Tarea 3.6 - Identificar los servicios de almacenamiento de AWS

### Pregunta 10
Una empresa guarda registros de auditoría que casi nunca consulta pero debe conservar durante 10 años al menor costo. ¿Qué clase de almacenamiento de S3 es la más adecuada?
- A) S3 Intelligent-Tiering
- B) S3 Glacier Deep Archive
- C) S3 One Zone-IA
- D) S3 Standard

---

## Tarea 3.7 - Identificar los servicios de IA/ML y de analítica de AWS

### Pregunta 11
¿Qué servicio convierte texto en voz realista?
- A) Amazon Textract
- B) Amazon Polly
- C) Amazon Transcribe
- D) Amazon Translate

---

## Tarea 3.8 - Identificar servicios de otras categorías de servicios de AWS dentro del alcance

### Pregunta 12
Una aplicación necesita desacoplar componentes enviando mensajes que se procesen de forma asíncrona. ¿Qué servicio es el más adecuado?
- A) Amazon SQS
- B) Amazon Macie
- C) AWS Shield
- D) Amazon Route 53

---

# Respuestas y Explicaciones

### Pregunta 1
**Respuesta correcta: B**
**Explicación:** La infraestructura como código permite definir y desplegar recursos de forma repetible y consistente. La consola manual es propensa a errores y no es repetible.

### Pregunta 2
**Respuesta correcta: C**
**Explicación:** Cada Región es un área geográfica con varias zonas de disponibilidad aisladas entre sí. Cada AZ está formada por uno o más centros de datos con energía y red independientes.

### Pregunta 3
**Respuesta correcta: D**
**Explicación:** CloudFront es una CDN que cachea contenido en ubicaciones de borde cercanas a los usuarios. Los demás servicios no ofrecen entrega global de contenido.

### Pregunta 4
**Respuesta correcta: D**
**Explicación:** Las instancias optimizadas para cómputo ofrecen procesadores de alto rendimiento y son ideales para cálculos intensivos. Las de memoria sirven para bases de datos en memoria y las de almacenamiento para alto IOPS.

### Pregunta 5
**Respuesta correcta: D**
**Explicación:** Lambda ejecuta código en respuesta a eventos y no requiere administrar servidores; se cobra por solicitud y duración. EC2, Outposts y Lightsail requieren administrar instancias o infraestructura.

### Pregunta 6
**Respuesta correcta: A**
**Explicación:** DynamoDB es una base de datos NoSQL clave-valor totalmente administrada y de baja latencia. RDS es relacional, Redshift es data warehouse y Neptune es de grafos.

### Pregunta 7
**Respuesta correcta: A**
**Explicación:** ElastiCache ofrece cachés en memoria (Redis/Valkey o Memcached) con latencia de microsegundos. Aurora es una base relacional, DMS migra datos y DocumentDB es una base de documentos.

### Pregunta 8
**Respuesta correcta: D**
**Explicación:** Los grupos de seguridad son firewalls con estado a nivel de instancia. Las Network ACL son sin estado y operan a nivel de subred. Las tablas de rutas y el internet gateway no filtran tráfico.

### Pregunta 9
**Respuesta correcta: D**
**Explicación:** Direct Connect establece una conexión de red dedicada hacia AWS. Route 53 es DNS, CloudFront es CDN y WAF es un firewall de aplicaciones.

### Pregunta 10
**Respuesta correcta: B**
**Explicación:** S3 Glacier Deep Archive es la clase de menor costo para datos de archivo con retención a largo plazo. S3 Standard es para acceso frecuente y las demás clases tienen mayor costo para este patrón.

### Pregunta 11
**Respuesta correcta: B**
**Explicación:** Amazon Polly convierte texto en voz. Transcribe hace lo contrario (voz a texto), Translate traduce idiomas y Textract extrae texto de documentos.

### Pregunta 12
**Respuesta correcta: A**
**Explicación:** SQS es un servicio de colas que desacopla los productores de los consumidores. SNS serviría para notificaciones pub/sub; los demás servicios no se usan para mensajería.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Dominio 3](../CLF-C02-Domains/CLF-C02-Domain-3.md) · [Siguiente: Dominio 4](../CLF-C02-Domains/CLF-C02-Domain-4.md)
