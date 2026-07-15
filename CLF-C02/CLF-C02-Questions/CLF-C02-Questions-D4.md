# Preguntas de Práctica - Dominio 4: Facturación, Precios y Soporte

**Navegación:** [Inicio](../README.md) · [Anterior: Dominio 4](../CLF-C02-Domains/CLF-C02-Domain-4.md) · [Siguiente: Índice de Servicios](../CLF_C02_Servicios.md)

---

## Tarea 4.1 - Comparar los modelos de precios de AWS

### Pregunta 1
Una carga de trabajo es tolerante a interrupciones y se ejecuta por lotes. ¿Qué opción de compra de EC2 ofrece el mayor ahorro?
- A) Dedicated Hosts
- B) Spot Instances
- C) On-Demand
- D) Capacity Reservations

---

### Pregunta 2
Una empresa ejecuta una aplicación estable durante varios años y puede comprometerse a un nivel de uso. ¿Qué opciones reducen el costo frente a On-Demand? (Seleccione DOS)
- A) Savings Plans
- B) Reserved Instances
- C) Instancias de corta duración
- D) Transferencia de datos de entrada
- E) Pago por cada solicitud

---

### Pregunta 3
¿Qué tráfico de datos entrante o saliente genera normalmente costo en AWS?
- A) Datos que entran a AWS desde internet
- B) Datos entre servicios dentro de una misma AZ siempre
- C) Datos entre instancias de la misma subred
- D) Datos que salen de AWS hacia internet

---

### Pregunta 4
Una empresa necesita cumplir requisitos de licenciamiento que exigen un servidor físico dedicado para su software. ¿Qué opción de EC2 debe usar?
- A) Instancias de ráfaga
- B) Savings Plans
- C) Spot Instances
- D) Dedicated Hosts

---

## Tarea 4.2 - Entender los recursos para facturación, presupuesto y administración de costos

### Pregunta 5
Una empresa desea recibir una alerta cuando el gasto mensual proyectado supere los USD 5.000. ¿Qué servicio debe usar?
- A) AWS Config
- B) AWS CloudTrail
- C) Amazon Inspector
- D) AWS Budgets

---

### Pregunta 6
¿Qué herramienta permite estimar el costo de una arquitectura **antes** de desplegarla?
- A) AWS Cost Explorer
- B) AWS Trusted Advisor
- C) AWS Pricing Calculator
- D) AWS Health Dashboard

---

### Pregunta 7
Una empresa con varias cuentas quiere recibir una sola factura y aprovechar los descuentos por volumen combinados. ¿Qué característica debe usar?
- A) Capa gratuita
- B) Etiquetas de asignación de costos
- C) AWS Cost and Usage Report
- D) Facturación consolidada de AWS Organizations

---

## Tarea 4.3 - Identificar los recursos técnicos y las opciones de AWS Support

### Pregunta 8
Una empresa necesita un Technical Account Manager (TAM) asignado y soporte proactivo para cargas críticas. ¿Qué plan de AWS Support debe elegir?
- A) Enterprise Support
- B) Basic Support
- C) Business Support+
- D) Developer Support

---

### Pregunta 9
¿Qué herramienta revisa la cuenta y entrega recomendaciones sobre costos, seguridad, rendimiento, tolerancia a fallos y límites de servicio?
- A) AWS Artifact
- B) AWS CloudTrail
- C) AWS Trusted Advisor
- D) AWS Control Tower

---

### Pregunta 10
Una empresa quiere encontrar software de terceros listo para desplegar y facturar el costo en su cuenta de AWS. ¿Qué servicio debe usar?
- A) AWS Marketplace
- B) AWS Prescriptive Guidance
- C) AWS re:Post
- D) AWS Support Center

---

# Respuestas y Explicaciones

### Pregunta 1
**Respuesta correcta: B**
**Explicación:** Las instancias Spot usan capacidad sobrante con descuentos de hasta el 90 %, pero AWS puede interrumpirlas. Son ideales para cargas flexibles y tolerantes a fallos.

### Pregunta 2
**Respuesta correcta: A, B**
**Explicación:** Los Savings Plans y las Reserved Instances ofrecen descuentos a cambio de un compromiso de uso a uno o tres años. Las demás opciones no son modelos de compromiso.

### Pregunta 3
**Respuesta correcta: D**
**Explicación:** La transferencia de datos hacia AWS suele ser gratuita, mientras que la transferencia saliente hacia internet y entre Regiones tiene costo.

### Pregunta 4
**Respuesta correcta: D**
**Explicación:** Los Dedicated Hosts ofrecen un servidor físico dedicado y visibilidad de sockets y núcleos, útil para licencias por socket o núcleo. Spot y Savings Plans son modelos de precio, no de aislamiento físico.

### Pregunta 5
**Respuesta correcta: D**
**Explicación:** AWS Budgets permite definir presupuestos y recibir alertas de gasto real o proyectado. Los demás servicios no administran presupuestos.

### Pregunta 6
**Respuesta correcta: C**
**Explicación:** AWS Pricing Calculator estima costos de arquitecturas planificadas. Cost Explorer analiza costos ya incurridos.

### Pregunta 7
**Respuesta correcta: D**
**Explicación:** La facturación consolidada de Organizations unifica la facturación de todas las cuentas y combina el uso para obtener descuentos por volumen. El CUR y las etiquetas sirven para analizar costos, no para consolidar la facturación.

### Pregunta 8
**Respuesta correcta: A**
**Explicación:** Enterprise Support incluye un TAM designado y orientación proactiva. Basic y Developer no lo incluyen, y Business Support+ ofrece soporte técnico 24/7 pero sin TAM designado.

### Pregunta 9
**Respuesta correcta: C**
**Explicación:** Trusted Advisor inspecciona el entorno y recomienda mejoras en varias categorías. CloudTrail audita llamadas a la API, Artifact entrega informes de cumplimiento y Control Tower configura una landing zone.

### Pregunta 10
**Respuesta correcta: A**
**Explicación:** AWS Marketplace es un catálogo digital de software de terceros con facturación integrada en AWS. Los otros recursos son de soporte y documentación técnica.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Dominio 4](../CLF-C02-Domains/CLF-C02-Domain-4.md) · [Siguiente: Índice de Servicios](../CLF_C02_Servicios.md)
