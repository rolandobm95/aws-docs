# Valor de la nube y AWS Well-Architected Framework (CLF-C02)

**Dominio relacionado:** Dominio 1 - Conceptos de la Nube (24 %)

---

## 1. Seis ventajas de la computación en la nube

| Ventaja | Idea clave |
|---|---|
| Cambiar CapEx por OpEx | Se paga por lo que se consume, sin inversión inicial |
| Economías de escala | AWS agrega el uso de muchos clientes y reduce los precios |
| Dejar de adivinar la capacidad | Se escala hacia arriba o hacia abajo según la demanda |
| Mayor velocidad y agilidad | Los recursos se aprovisionan en minutos |
| Dejar de gastar en centros de datos | El equipo se enfoca en el negocio, no en la infraestructura |
| Alcance global en minutos | Se despliega en varias Regiones con pocos clics |

---

## 2. Conceptos que se confunden

| Concepto | Significado | Ejemplo |
|---|---|---|
| Escalabilidad | Capacidad de crecer para soportar más carga | Pasar de 2 a 20 instancias |
| Elasticidad | Crecer y reducir automáticamente según la demanda | Auto Scaling |
| Agilidad | Probar e implementar rápidamente | Lanzar un entorno en minutos |
| Alta disponibilidad | Minimizar el tiempo de inactividad | Multi-AZ |
| Tolerancia a fallos | Seguir operando sin interrupción aunque falle un componente | Componentes redundantes |

---

## 3. Modelos de servicio y despliegue

| Modelo | Qué administra el cliente | Ejemplo |
|---|---|---|
| IaaS | Sistema operativo, aplicaciones y datos | Amazon EC2 |
| PaaS | Aplicaciones y datos | AWS Elastic Beanstalk |
| SaaS | Solo el uso del servicio | Amazon Connect |

| Despliegue | Descripción |
|---|---|
| Nube | Todo corre en la nube |
| Híbrido | Se combinan recursos on-premises y en la nube (por ejemplo, AWS Outposts, Direct Connect) |
| On-premises | Todo corre en el centro de datos propio |

---

## 4. AWS Well-Architected Framework

| Pilar | Objetivo | Palabra clave |
|---|---|---|
| Excelencia operativa | Ejecutar y monitorear sistemas y mejorar procesos | Automatizar, mejorar continuamente |
| Seguridad | Proteger información, sistemas y activos | Mínimo privilegio, cifrado |
| Confiabilidad | Recuperarse de fallos y cumplir la demanda | Multi-AZ, recuperación |
| Eficiencia del rendimiento | Usar recursos de forma eficiente | Elegir el recurso correcto |
| Optimización de costos | Evitar gastos innecesarios | Pagar solo lo que se usa |
| Sostenibilidad | Minimizar el impacto ambiental | Eficiencia energética |

> **Regla clave:** una misma decisión puede afectar a varios pilares. Por ejemplo, Multi-AZ mejora la confiabilidad pero aumenta el costo.

AWS Well-Architected Tool es el servicio que permite revisar cargas de trabajo frente a estas mejores prácticas.

---

## 5. Migración y AWS CAF

### Estrategias de migración (7 R)
| Estrategia | Descripción |
|---|---|
| Retire | Apagar lo que ya no se necesita |
| Retain | Mantener en el entorno actual |
| Rehost | Mover sin cambios (lift and shift) |
| Relocate | Mover a la nube sin cambios de hipervisor (por ejemplo, VMware) |
| Repurchase | Cambiar a un producto distinto (por ejemplo, SaaS) |
| Replatform | Pequeños ajustes para aprovechar la nube |
| Refactor | Rediseñar la aplicación |

### Herramientas
| Necesidad | Servicio |
|---|---|
| Descubrir servidores locales | AWS Application Discovery Service |
| Rehost de servidores | AWS Application Migration Service |
| Seguimiento de migración | AWS Migration Hub |
| Caso de negocio | Migration Evaluator |
| Migrar datos de una base | AWS DMS |
| Convertir el esquema entre motores distintos | AWS SCT |

### AWS CAF
Organiza la adopción de la nube en perspectivas: negocio, personas, gobernanza, plataforma, seguridad y operaciones. Beneficios: menor riesgo de negocio, mejor desempeño ESG, mayores ingresos y mayor eficiencia operativa.

---

## 6. Economía de la nube

- Costos fijos: no cambian con el uso. Costos variables: cambian con el consumo.
- Costos on-premises: hardware, energía, enfriamiento, espacio, personal y renovación tecnológica.
- Licencias: BYOL (se trae la licencia propia) frente a licencia incluida.
- Rightsizing: ajustar el tamaño de los recursos a la demanda real.
- Automatización: reduce errores y costos operativos.

---

## Checklist final

- [ ] Enumerar las seis ventajas de la nube.
- [ ] Diferenciar elasticidad, escalabilidad y alta disponibilidad.
- [ ] Nombrar los seis pilares y su objetivo.
- [ ] Identificar una estrategia de migración a partir de un escenario.
- [ ] Explicar costos fijos frente a variables y BYOL frente a licencia incluida.

---

**Navegación:** [Inicio](../README.md) · [Siguiente: Responsabilidad compartida y seguridad](02-Shared-Responsibility-and-Security.md)
