# Preguntas de Práctica - Dominio 1: Conceptos de la Nube

**Navegación:** [Inicio](../README.md) · [Anterior: Dominio 1](../CLF-C02-Domains/CLF-C02-Domain-1.md) · [Siguiente: Dominio 2](../CLF-C02-Domains/CLF-C02-Domain-2.md)

---

## Tarea 1.1 - Definir los beneficios de la nube de AWS

### Pregunta 1
Una empresa de comercio electrónico espera un pico de tráfico durante una campaña de temporada y no quiere comprar servidores que queden ociosos después. ¿Qué beneficio de la nube de AWS responde mejor a esta necesidad?
- A) Elasticidad: aumentar y reducir recursos según la demanda.
- B) Latencia cero: servir contenido sin retardo de red.
- C) Cumplimiento: transferir la seguridad de los datos a AWS.
- D) Tolerancia a fallos: eliminar cualquier punto único de fallo.

---

### Pregunta 2
¿Cuál de las siguientes opciones es una ventaja de la nube de AWS frente a un centro de datos propio?
- A) Cambiar gasto de capital (CapEx) por gasto variable (OpEx).
- B) Pagar siempre una tarifa mensual fija sin importar el uso.
- C) Administrar físicamente el hardware de los servidores.
- D) Disponer de capacidad fija estimada con un año de anticipación.

---

### Pregunta 3
Una empresa quiere que su aplicación siga disponible aunque falle un centro de datos completo dentro de una Región. ¿Qué enfoque debe usar?
- A) Desplegar la aplicación en varias zonas de disponibilidad.
- B) Desplegar la aplicación en una sola zona de disponibilidad con una instancia grande.
- C) Usar únicamente una ubicación de borde.
- D) Aumentar el tamaño del volumen de almacenamiento.

---

## Tarea 1.2 - Identificar los principios de diseño de la nube de AWS

### Pregunta 4
¿Qué pilar del AWS Well-Architected Framework se enfoca en ejecutar y monitorear sistemas, y en mejorar continuamente los procesos y procedimientos?
- A) Excelencia operativa
- B) Confiabilidad
- C) Sostenibilidad
- D) Seguridad

---

### Pregunta 5
Una empresa revisa su arquitectura para reducir la huella de carbono y el consumo energético de su carga de trabajo. ¿Qué pilar del Well-Architected Framework está evaluando?
- A) Eficiencia del rendimiento
- B) Optimización de costos
- C) Excelencia operativa
- D) Sostenibilidad

---

## Tarea 1.3 - Entender los beneficios y estrategias de migración a la nube de AWS

### Pregunta 6
Una empresa quiere migrar sus servidores a AWS sin modificar el código de las aplicaciones ("lift and shift"). ¿Qué estrategia de migración describe esto?
- A) Repurchase
- B) Rehost
- C) Refactor
- D) Retire

---

### Pregunta 7
¿Qué recurso de AWS ayuda a las organizaciones a identificar brechas de habilidades y procesos mediante perspectivas de negocio y de tecnología para planificar su transformación en la nube?
- A) AWS Pricing Calculator
- B) AWS Health Dashboard
- C) AWS Trusted Advisor
- D) AWS Cloud Adoption Framework (AWS CAF)

---

### Pregunta 8
Una empresa necesita migrar una base de datos Oracle a Amazon Aurora PostgreSQL. ¿Qué par de servicios debe usar? 
- A) Amazon Athena y AWS Glue
- B) AWS DMS y AWS SCT
- C) AWS Backup y AWS Config
- D) AWS Snowball y Amazon S3

---

## Tarea 1.4 - Entender los conceptos de economía de la nube

### Pregunta 9
¿Cuál es la diferencia principal entre costos fijos y costos variables en la nube?
- A) Los variables solo existen en entornos on-premises.
- B) Los fijos no cambian con el uso; los variables cambian según el consumo.
- C) Los fijos dependen del consumo y los variables no.
- D) Ambos son iguales en AWS.

---

### Pregunta 10
Una empresa descubre que sus instancias EC2 usan menos del 10 % de CPU. ¿Qué práctica debería aplicar para reducir costos?
- A) Comprar más instancias para tener capacidad extra.
- B) Rightsizing: elegir un tamaño de instancia acorde con la carga.
- C) Cambiar a una Región más lejana.
- D) Migrar a un centro de datos propio.

---

# Respuestas y Explicaciones

### Pregunta 1
**Respuesta correcta: A**
**Explicación:** La elasticidad permite aprovisionar recursos cuando la demanda sube y liberarlos cuando baja, pagando solo por lo usado. La tolerancia a fallos es otro concepto distinto. Transferir toda la seguridad a AWS es incorrecto porque la seguridad **en** la nube sigue siendo responsabilidad del cliente. La latencia cero no es posible.

### Pregunta 2
**Respuesta correcta: A**
**Explicación:** Una de las seis ventajas de la nube es reemplazar la inversión inicial (CapEx) por costos variables (OpEx) que se pagan según el consumo. Las demás opciones describen justamente el modelo on-premises tradicional.

### Pregunta 3
**Respuesta correcta: A**
**Explicación:** Cada zona de disponibilidad está aislada y no comparte puntos únicos de fallo con las demás; distribuir la aplicación en varias AZ logra alta disponibilidad. Una sola AZ sigue siendo un punto único de fallo. Las ubicaciones de borde sirven para entregar contenido, no para alojar la aplicación completa. El tamaño del volumen no mejora la disponibilidad.

### Pregunta 4
**Respuesta correcta: A**
**Explicación:** El pilar de excelencia operativa cubre la ejecución y monitoreo de cargas de trabajo y la mejora continua de procesos. Seguridad protege datos y sistemas; Confiabilidad se centra en recuperarse de fallos; Sostenibilidad minimiza el impacto ambiental.

### Pregunta 5
**Respuesta correcta: D**
**Explicación:** El pilar de sostenibilidad se enfoca en minimizar el impacto ambiental de las cargas de trabajo en la nube. Optimización de costos busca evitar gastos innecesarios y Eficiencia del rendimiento usa recursos de cómputo de forma eficiente, pero ninguno apunta directamente a la huella ambiental.

### Pregunta 6
**Respuesta correcta: B**
**Explicación:** Rehost (lift and shift) mueve las aplicaciones a la nube sin cambios significativos. Refactor reescribe la aplicación; Repurchase cambia a un producto distinto (por ejemplo, SaaS); Retire apaga lo que ya no se necesita.

### Pregunta 7
**Respuesta correcta: D**
**Explicación:** AWS CAF organiza la guía de adopción en perspectivas (negocio, personas, gobernanza, plataforma, seguridad y operaciones) para ayudar a planificar la transformación. Pricing Calculator estima costos, Trusted Advisor da recomendaciones de buenas prácticas y Health Dashboard informa del estado de los servicios.

### Pregunta 8
**Respuesta correcta: B**
**Explicación:** AWS SCT convierte el esquema y el código de una base de datos a otro motor, y AWS DMS migra y replica los datos. Las demás combinaciones no están orientadas a migrar bases de datos heterogéneas.

### Pregunta 9
**Respuesta correcta: B**
**Explicación:** Un costo fijo no cambia con el uso (por ejemplo, comprar un servidor), mientras que un costo variable crece o disminuye según el consumo, como ocurre con el pago por uso de AWS.

### Pregunta 10
**Respuesta correcta: B**
**Explicación:** El rightsizing ajusta el tamaño de los recursos a la demanda real y evita pagar capacidad que no se usa. AWS Compute Optimizer entrega recomendaciones de este tipo. Las demás opciones aumentan el costo o no resuelven el sobredimensionamiento.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Dominio 1](../CLF-C02-Domains/CLF-C02-Domain-1.md) · [Siguiente: Dominio 2](../CLF-C02-Domains/CLF-C02-Domain-2.md)
