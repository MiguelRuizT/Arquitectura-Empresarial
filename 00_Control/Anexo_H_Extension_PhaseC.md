# Anexo H-C · Hipótesis adicionales de enseñanza para Phase C

**Proyecto:** TG-EA-OMA-2026 · Fecha: 30/10/2026 · Versión: 2.0 · Estado: Draft.

Este anexo no altera H-01..H-22 del expediente original. Se crea para que los datos ilustrativos añadidos en las fases de arquitectura de datos y aplicaciones sean **auditables, repetibles y explícitamente hipotéticos**. Los términos WMS, QA, ERP, IoT y las claves de ejemplo **no describen inventarios ni códigos reales de T&G Global**.

| ID | Tema | Dato aceptado solo en el escenario | Criterio de validación futura |
|---|---|---|---|
| H-C23 | Fuente y aplicaciones | WMS Packing, QA Registry, ERP Export y hoja puente son nombres lógicos del ejercicio. IoT/OT es una hipótesis no verificada. | Descubrimiento de aplicaciones y propietarios |
| H-C24 | Identidad | LotId persistente, SourceMapping enlaza claves locales y LotGenealogy conserva padres/hijos en split/merge. | Muestras de equivalencia con Calidad |
| H-C25 | Evento | EventId, LotId, EventType, OccurredAtUTC, CapturedAtUTC, SourceSystem, ActorRole, RuleVersion, EvidenceRef y CorrelationId. | Validación del contrato del evento |
| H-C26 | Interoperabilidad | Adapters de fuentes, contrato común, Traceability Component y consulta autorizada; sin producto tecnológico elegido. | Contrato revisado por IT/OT |
| H-C27 | Data Quality | Metas propuestas: 100% unicidad LotId; ≥99% eventos críticos completos; ≥99% aristas genealógicas válidas; 0 cierres silenciosos. | Aprobar numerador, denominador, muestra y umbral |
| H-C28 | Gobierno | Calidad posee semántica de identidad y autoridad de liberación; Gobierno de Datos es steward; IT/OT integra, pero no libera lotes. | Aprobación RACI y segregación |
| H-C29 | Continuidad | Consulta objetivo ≥99,5% (ya en H-08); recepción tolera caídas e idempotencia. RTO/RPO por definir. | Ensayo y decisión Phase D |
| H-C30 | Interfaces | IF-01..07 son **contratos lógicos**, no endpoints o soluciones instaladas. | Aceptación por emisor/consumidor |
| H-C31 | Impacto ilustrativo | 20 000 cajas/día × 6% × NZD 4/caja = NZD 4 800/día. **NZD = dólar neozelandés.** | No usar como ROI ni dato corporativo |
| H-C32 | Estados | Baseline docente, Target propuesto y Roadmap candidato; gate sin aprobar. | Control de versiones y decisiones |

## Reglas de uso

1. No mezclar los supuestos H-C con la evidencia pública de T&G Global. Los comunicados empresariales solo soportan contexto general de cadena y Whakatū.
2. Si un equipo decide cambiar un supuesto, registre cambio de versión y actualice **ADD, ARS, catálogos, vistas, trazabilidad y Roadmap**.
3. No asignar una marca comercial ni una topología de red a Phase C.
4. El resultado de negocio `BSV-03 Liberación conforme` es una responsabilidad de **Calidad**; un servicio o contratista técnico puede proporcionar información pero no obtener de ese hecho autoridad para liberar lotes.
5. Mantener la referencia `H-08` para los tres KPIs originales: **≥94%** lotes con historial, **<30 minutos** de consulta y **≥99,5%** disponibilidad de servicio.

La versión tabular editable de H-C23..32 está en la pestaña `Supuestos_HC` del libro `C3_Integracion_Traceability_Viewpoints_Gobierno_v2.0.xlsx`.
