# CHANGELOG · SI605 · Grupo 03 · Beta · Architecture Repository

Formato: versión · fecha · responsable · cambio · fundamento · artefactos.

## v0.3 · PC3 · 26/11/2026

### Reorganización del repositorio (guía PC3 §4.1 y §4.2)
| ID | Cambio | Fundamento | Artefactos |
|---|---|---|---|
| CHG-R01 | Estructura 00 a 11 de la guía (antes: 00_Control vacío, 01–05 por fase, 06_Architecture_Repository y 07_Enterprise_Continuum vacíos) | Guía §4.1 | Todo el ZIP |
| CHG-R02 | Nuevos README.md, MANIFEST.xlsx y CHANGELOG.md en la raíz | Guía §4.2 (archivos obligatorios) | Raíz |
| CHG-R03 | Fase C separada en `04_Phase_C_Data` y `05_Phase_C_Application`; los entregables comunes C-00..C-06 y C3 se guardan una sola vez en `04/00_Comun_Fase_C` | Guía §4.1 · evitar copias | C-00..C-06, C1, C2, C3 |
| CHG-R04 | Versiones anteriores movidas a `_historico/` (C2 v0.1, T1 v0.1, T2 v0.1, B-07 matriz v0.1, XML originales D) | «No borrar historia» (guía §4.2) | `_historico/` |
| CHG-R05 | `PC3_Cap01_Continuidad_desde_PC2_v0.1.docx` sale de `05_Phase_D` y pasa a `07_Entregables_Integrados/Informe_PC3_Secciones/` | Estaba en la fase equivocada | Cap. 1 |
| CHG-R06 | `Explicacion_B-02_a_B-05_v1.3_revisada.docx` sale del entregable (material de estudio) | No es artefacto de arquitectura | B |
| CHG-R07 | Se descarta `06_Governance_Repository_Error.txt` (error de descarga de Google Drive). Su contenido se reconstruye en `00-01` con B-07 v1.2 y el expediente PRE-A v0.3 | El Governance Repository no se descargó | 00-01 |

### Modelo ArchiMate (guía Actividad J)
| ID | Cambio | Fundamento | Artefactos |
|---|---|---|---|
| CHG-M01 | Un solo modelo integrado B/C/D (211 elementos, 257 relaciones, 20 vistas) en XML Open Exchange y `.archimate` | Guía §2 Act. J: «modelo único» | 08 |
| CHG-M02 | 20 vistas exportadas a SVG | Guía §4.2: SVG/PNG | 08/Vistas_SVG |
| CHG-M03 | XML de la Fase D corregidos (v0.2): tipos `XxxRelationship`/`UsedBy` → tipos Open Exchange; `&` sin escapar en T-V01; nodos y conexiones sin `xsi:type`; 19 relaciones no válidas en ArchiMate 3.1 | Los XML originales no importaban en Archi | T-V01..T-V10, X-V02 |
| CHG-M04 | Unificación de IDs duplicados entre bloques (BSV, AC, AS, APP-05, DO, objetos de negocio). Autoridad: B-06 y C1/C2 | «IDs no se contradicen» (guía §4.2) | 08-01 › Unificacion_IDs |

### Registros consolidados (guía Actividades I y K)
| ID | Cambio | Artefactos |
|---|---|---|
| CHG-I01 | Gap Register único: 19 gaps (5 GAP-B, 3 GAP-D, 3 GAP-A, 8 GAP-T) | 07-01 |
| CHG-I02 | ARS consolidada REQ → AR → NFR-T y Success Measures | 07-01 |
| CHG-I03 | CRC → D-RC/A-RC → T-RC con dependencias | 07-01 |
| CHG-I04 | Decision Log con numeración única DEC-01..DEC-29; alias DEC-C/TD-DEC de §9.4 mapeados | 00-01 |
| CHG-I05 | Gates PRE→A, A→B, B→C, C→D y D→E en una sola hoja; Gate D→E **pendiente de decisión** | 00-01 |
| CHG-I06 | ADD/ARS consolidados como índice único B+C+D | 07-02 |
| CHG-I07 | Dossier de evidencia, supuestos SV, plan NV y registro de uso de IA | 09-01 |
| CHG-I08 | Índice de plantillas TOGAF y aplicabilidad M/S de artefactos C/D | 10-01 |
| CHG-I09 | Índice de evidencia de las dos cadenas E2E con rutas reales | 11-01 |

### Cambios de PC2 → PC3 en el contenido
Se documentan en `07_Entregables_Integrados/Informe_PC3_Secciones/PC3_Cap01_Continuidad_desde_PC2_v0.1.docx` (REV-01 a REV-07) y en `C-00 › Change_Log` (CHG-C01..), `C3 › Change_Log_C` (CHG-C08..) y T-00 (CHG-D..).

## v0.2 · PC2 · 10/11/2026
Phase B completa (B-01 a B-09), revisión de Preliminary y Phase A (v1.1–v1.3), Decision Log DEC-07..DEC-14, Risk Log RSK-07..RSK-11, gate B → C con condiciones (DEC-14).

## v0.1 · PC1 · 09/10/2026
Expediente PRE-A: PRE-01..PRE-06, A-01..A-06, vistas VIEW-05..VIEW-08, Decision Log DEC-01..DEC-06, Risk Log RSK-01..RSK-06.
