# Precios, facturación y soporte (CLF-C02)

**Dominio relacionado:** Dominio 4 - Facturación, Precios y Soporte (12 %)

---

## 1. Principios de precios

- Pago por uso: se paga solo por lo que se consume.
- Pagar menos al reservar: los compromisos reducen el precio.
- Pagar menos al usar más: los precios por volumen disminuyen con el uso.
- Capa gratuita (Free Tier): ofertas gratuitas, de prueba o de 12 meses según el servicio.

---

## 2. Modelos de compra de cómputo

| Modelo | Descripción | Ideal para |
|---|---|---|
| On-Demand | Pago por segundo u hora, sin compromiso | Cargas impredecibles o de corto plazo |
| Reserved Instances | Compromiso de 1 o 3 años con descuento | Cargas estables |
| Savings Plans | Compromiso de gasto por hora a 1 o 3 años | Cargas estables con flexibilidad |
| Spot Instances | Capacidad sobrante con gran descuento, puede interrumpirse | Cargas tolerantes a interrupciones |
| Dedicated Hosts | Servidor físico dedicado | Licencias por socket/núcleo y cumplimiento |
| Dedicated Instances | Instancias en hardware de un solo cliente | Aislamiento de hardware |
| Capacity Reservations | Reserva de capacidad en una AZ | Garantizar capacidad |

- Reserved Instances: Standard (mayor descuento) y Convertible (más flexibilidad).
- En AWS Organizations, los descuentos de RI y Savings Plans pueden compartirse entre las cuentas de la organización.

---

## 3. Transferencia de datos

| Tráfico | Costo habitual |
|---|---|
| Entrada desde internet | Gratuito |
| Salida hacia internet | Con costo |
| Entre Regiones | Con costo |
| Dentro de la misma AZ (IP privada) | Normalmente sin costo |
| Entre AZ de una Región | Normalmente con costo |

---

## 4. Herramientas de costos

| Necesidad | Herramienta |
|---|---|
| Estimar costos antes de desplegar | AWS Pricing Calculator |
| Analizar y pronosticar costos pasados | AWS Cost Explorer |
| Definir presupuestos y alertas | AWS Budgets |
| Datos de costo y uso más detallados | AWS Cost and Usage Report |
| Detectar gastos inusuales | AWS Cost Anomaly Detection |
| Un solo pago y descuentos por volumen | Facturación consolidada (AWS Organizations) |
| Asignar costos por proyecto o equipo | Etiquetas de asignación de costos |
| Recomendaciones de rightsizing | AWS Compute Optimizer |

### Etiquetas de asignación de costos
- Definidas por AWS (por ejemplo, `aws:createdBy`) y definidas por el usuario (por ejemplo, `Proyecto`).
- Deben activarse en Billing and Cost Management para aparecer en los reportes, como el Cost and Usage Report.

---

## 5. AWS Support

Según la guía vigente, los planes son: **Basic Support**, **Business Support+**, **Enterprise Support** y **Unified Operations**. Los planes históricos incluyen Developer, Business y Enterprise On-Ramp.

| Característica | Basic | Planes de pago |
|---|---|---|
| Atención al cliente y comunidades | Sí | Sí |
| Documentación, whitepapers y foros | Sí | Sí |
| AWS Trusted Advisor | Comprobaciones básicas | Conjunto ampliado según el plan |
| AWS Health Dashboard | Sí | Sí |
| Soporte técnico por casos | No | Sí |
| Technical Account Manager (TAM) | No | Planes de nivel Enterprise |

> **Regla clave:** un TAM asignado se asocia con los planes de nivel Enterprise.

---

## 6. Recursos técnicos y asistencia

| Recurso | Descripción |
|---|---|
| AWS Documentation, Whitepapers y Blogs | Fuentes oficiales |
| AWS Prescriptive Guidance | Estrategias y patrones probados |
| AWS Knowledge Center | Preguntas frecuentes de soporte |
| AWS re:Post | Comunidad de preguntas y respuestas |
| AWS Trusted Advisor | Recomendaciones de costos, seguridad, rendimiento, tolerancia a fallos y límites |
| AWS Health Dashboard / Health API | Estado y eventos que afectan tus recursos |
| AWS Trust and Safety | Reportar abuso de recursos de AWS |
| AWS Professional Services | Consultoría de AWS |
| Arquitectos de soluciones | Orientación de arquitectura |
| AWS Partner Network (APN) | Socios: ISV e integradores de sistemas |
| AWS Marketplace | Catálogo de software de terceros |

Beneficios de ser socio de AWS: capacitación y certificación, eventos y descuentos por volumen.

---

## Checklist final

- [ ] Elegir el modelo de compra de EC2 correcto a partir de un escenario.
- [ ] Diferenciar Pricing Calculator, Cost Explorer, Budgets y CUR.
- [ ] Explicar facturación consolidada y etiquetas de asignación de costos.
- [ ] Reconocer qué plan de soporte incluye un TAM.
- [ ] Ubicar el recurso adecuado: Knowledge Center, re:Post, Prescriptive Guidance o Trusted Advisor.

---

**Navegación:** [Inicio](../README.md) · [Anterior: Comparativa de servicios](03-Core-Services-Comparison.md)
