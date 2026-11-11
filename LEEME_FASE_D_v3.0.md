# Repositorio T&G — ADM Preliminary, A, B, C, D · v3.0

Caso didáctico hipotético | UNI · SI605 Arquitectura Empresarial | 06/11/2026.

## Estructura acumulativa

- `00_Control` a `09_Phase_C_Guia_Repositorio`: **fuentes originales v2.0 preservadas**, no se sustituyen los documentos y las 15 vistas anteriores.
- `10_Phase_D_Entregables_TOGAF`: 10 documentos (incluye plantilla oficial The Open Group Phase C/D completada, ADD, requisitos refinados, roadmap candidato, ABB, ciberseguridad, 5 ejemplos y handoff).
- `11_Phase_D_Catalogos_Matrices`: dos Excel con 18 pestañas, catálogos estándares/tecnología, matriz aplicación-tecnología, datos-tecnología, NFR, gaps, principios, roadmap, conduits, decisiones y trazabilidad.
- `12_Phase_D_Vistas_ArchiMate`: XML combinado Preliminary/A/B/C/D con 26 vistas y 11 XML individuales de Phase D, más 11 SVG ilustrativos. Abrir en Archi con ArchiMate Model Exchange File import. *El SVG es figura de apoyo, el XML es editable en Archi.*
- `13_Phase_D_Soporte_Docente`: orientación de práctica de dos horas y referencias cruzadas.

## Artefactos Phase D recomendados por plantilla oficial Open Group 10 (julio 2024)

1. Technology Standards Catalog — T1 pestaña 01.
2. Technology Portfolio Catalog — T1 pestaña 02.
3. Application/Technology Matrix — T1 pestaña 08.
4. Environments and Locations Diagram — T-V01, T-V02.
5. Platform Decomposition Diagram — T-V03, T-V06.
6. Processing Diagram — T-V04.
7. Networked Computing/Hardware Diagram — T-V05.
8. Network and Communications Diagram — T-V07.

**Además**: principios refinados T1/03; NFR T1/04; gaps T1/05; candidatos de Architecture Roadmap T1/06; decisiones T1/07; Security T1/10; rutas y criterios a Phase E en T-09. Es importante distinguir una *plantilla recomendada* de la lista global de *salidas del ADM*.

## Instrucciones Archi

1. Archi → File → Import → Open Exchange File → seleccionar `TG_ADM_Preliminary_PhaseA_PhaseB_PhaseC_PhaseD_26Views_OpenExchange_v3.0.xml`.
2. Las 15 vistas previas se conservan; las 11 vistas nuevas utilizan prefijos `T-V01`...`T-V10` y `X-V02`.
3. Guardar como modelo `.archimate` nativo de Archi si se desea. Nunca editar el XML en Excel.

**Precaución**: importación validada a nivel XML/referencias, no se declara haber abierto en una instalación real de Archi. Al importar revisar la disposición automática de conexiones y estilos, según versión de Archi.

Todos los nombres y cifras de arquitectura empresarial T&G son supuestos pedagógicos; validar en empresa antes de cualquier ejecución.
