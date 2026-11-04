# AWS Docs

Documentación de referencia y material de estudio sobre servicios y arquitecturas de AWS, en español. El repositorio reúne guías por servicio, diagramas de arquitectura, infografías y guías de preparación para certificaciones de AWS.

---

## Contenido

| Carpeta | Descripción |
|---------|-------------|
| [`Docs-Services/`](Docs-Services) | Documentación general por categoría de servicio AWS (cómputo, bases de datos, redes, seguridad, etc.). Guías de referencia con conceptos, casos de uso y matrices de decisión. |
| [`Documentation/`](Documentation) | Notas temáticas transversales: recuperación ante desastres e interconexión de redes. |
| [`Architectures-Diagrams/`](Architectures-Diagrams) | Diagramas de arquitectura de ejemplo por categoría de servicio (PNG). |
| [`Docs-Diagrams/`](Docs-Diagrams) | Diagramas de apoyo a la documentación: PrivateLink, Transit Gateway, VPC Peering y estrategias de DR. |
| [`Infographics/`](Infographics) | Infografías de servicios individuales, organizadas por categoría. |
| [`SAA-C03/`](SAA-C03/README.md) | Guía de estudio para el examen AWS Certified Solutions Architect – Associate (SAA-C03). |
| [`CLF-C02/`](CLF-C02/README.md) | Guía de estudio para el examen AWS Certified Cloud Practitioner (CLF-C02). |

---

## Documentación por servicio

`Docs-Services/` contiene una guía por cada categoría de servicio de AWS. Cada documento incluye el alcance de la categoría, conceptos por servicio, casos de uso, errores comunes, una matriz de decisión y referencias oficiales.

| # | Categoría |
|---|-----------|
| 01 | [Análisis](Docs-Services/01-Analytics.md) |
| 02 | [Integración de aplicaciones](Docs-Services/02-Application-Integration.md) |
| 03 | [Administración de costos](Docs-Services/03-AWS-Cost-Management.md) |
| 04 | [Cómputo](Docs-Services/04-Compute.md) |
| 05 | [Contenedores](Docs-Services/05-Containers.md) |
| 06 | [Bases de datos](Docs-Services/06-Database.md) |
| 07 | [Herramientas para desarrolladores](Docs-Services/07-Developer-Tools.md) |
| 08 | [Frontend web y móvil](Docs-Services/08-Front-End-Web-and-Mobile.md) |
| 09 | [Machine Learning](Docs-Services/09-Machine-Learning.md) |
| 10 | [Administración y gobernanza](Docs-Services/10-Management-and-Governance.md) |
| 11 | [Servicios multimedia](Docs-Services/11-Media-Services.md) |
| 12 | [Migración y transferencia](Docs-Services/12-Migration-and-Transfer.md) |
| 13 | [Redes y entrega de contenido](Docs-Services/13-Networking-and-Content-Delivery.md) |
| 14 | [Seguridad, identidad y cumplimiento](Docs-Services/14-Security-Identity-and-Compliance.md) |
| 15 | [Sin servidor](Docs-Services/15-Serverless.md) |
| 16 | [Almacenamiento](Docs-Services/16-Storage.md) |

---

## Guías de certificación

### AWS Certified Cloud Practitioner (CLF-C02)
Nivel fundacional. Cubre conceptos de la nube, seguridad y cumplimiento, tecnología y servicios, y facturación, precios y soporte.

- [Guía CLF-C02](CLF-C02/README.md)

| Dominio | Peso |
|---------|------|
| Conceptos de la Nube | 24% |
| Seguridad y Cumplimiento | 30% |
| Tecnología y Servicios de la Nube | 34% |
| Facturación, Precios y Soporte | 12% |

### AWS Certified Solutions Architect – Associate (SAA-C03)
Nivel asociado. Cubre el diseño de arquitecturas seguras, resilientes, de alto rendimiento y optimizadas en costos.

- [Guía SAA-C03](SAA-C03/README.md)

| Dominio | Peso |
|---------|------|
| Diseño de Arquitecturas Seguras | 30% |
| Diseño de Arquitecturas Resistentes | 26% |
| Diseño de Arquitecturas de Alto Rendimiento | 24% |
| Diseño de Arquitecturas con Optimización de Costos | 20% |

Cada guía incluye documentos por dominio, preguntas de práctica, notas de repaso y un índice de servicios dentro del alcance del examen.

---

## Cómo usar este repositorio

- Para **consultar un servicio concreto**, empieza por `Docs-Services/`.
- Para **preparar una certificación**, abre el `README.md` de la guía correspondiente (`CLF-C02/` o `SAA-C03/`) y sigue la navegación de los documentos.
- Para **apoyarte en diagramas**, revisa `Architectures-Diagrams/`, `Docs-Diagrams/` e `Infographics/`.

---

## Recursos oficiales de AWS

- [Documentación de AWS](https://docs.aws.amazon.com/)
- [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/)
- [AWS Architecture Center](https://aws.amazon.com/architecture/)
- [AWS Skill Builder](https://explore.skillbuilder.aws/)
- [AWS Certification](https://aws.amazon.com/certification/)

---

> Las guías de certificación son material de estudio no oficial. Los pesos y dominios se basan en las guías oficiales de examen de AWS, que pueden cambiar; verifica siempre la versión vigente en el sitio de AWS.
