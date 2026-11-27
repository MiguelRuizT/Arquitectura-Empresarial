# SI605 PC3 · Grupo 03 · Architecture Repository v0.3

**Empresa:** Complejo Agroindustrial Beta S.A. (caso académico; los datos internos no verificados se marcan NV)
**Value stream (único, igual que PC1 y PC2):** «Asegurar arándano exportable: desde cosecha hasta despacho refrigerado» (etapas E1 a E7)
**Alcance ADM:** Preliminary, Phase A y Phase B revisadas + Phase C (Datos y Aplicaciones) + Phase D (Tecnología), con Requirements Management transversal.
**Versión del expediente:** v0.3 · 26/11/2026 · Estado: Draft para entrega PC3
**Curso:** SI605 Arquitectura Empresarial · FIIS–UNI · 2026-II

## Equipo

| Integrante | Nombre | Bloque PC3 |
|---|---|---|
| Int. 1 | Jens Herrera | 4.4–5.7 |
| Int. 2 | Cristhian Maturrano | 8.5–10.3 |
| Int. 3 | Julio Rubén Ortiz De Orue Huamani | 6.1–7.3 |
| Int. 4 | Miguel Ruiz Tacas | 7.4–8.4 |
| Int. 5 | Jesús Carhuas Bastidas | 3.4–4.3 |
| Int. 6 | Pedro Pablo Huacanjulca | 2.1–3.3 |

## Cómo abrir el expediente

1. Empieza por **`MANIFEST.xlsx`**: lista el 100 % de los archivos con ID, fase, tipo, owner, versión, estado y ruta.
2. **`CHANGELOG.md`** resume qué cambió de PC1 → PC2 → PC3 y por qué.
3. El **modelo ArchiMate** está en `08_ArchiMate_Modelos/` (XML Open Exchange + `.archimate` de Archi + 20 vistas SVG). Instrucciones en su `LEEME.md`.
4. Los **registros únicos** (Decision Log, Risk Log, Gates, Standards, Continuum) están en `00_Control_Gobierno/`, y el **Gap Register, la ARS, los CRC y la trazabilidad consolidados** en `07_Entregables_Integrados/`.
5. Para la sustentación, `11_Sustentacion/11-01_Indice_Evidencia_Sustentacion_v0.3.xlsx` recorre las dos cadenas E2E con la ruta de cada ID.

Los `.docx` se abren con Word; los `.xlsx` con Excel; el `.archimate` con Archi 4.x/5.x.

## Índice de carpetas

| Carpeta | Contenido |
|---|---|
| `00_Control_Gobierno/` | `00-01_Registro_Gobierno_v0.3.xlsx`: control de versiones, equipo, Capability Charter, gates PRE→A … D→E, Decision Log DEC-01..29, Risk Log, standards, convenciones de ID, Enterprise Continuum y glosario |
| `01_Preliminary/` | PRE-01 a PRE-06 |
| `02_Phase_A_Architecture_Vision/` | A-01 a A-06 |
| `03_Phase_B_Business/` | B-01 a B-09 (docx + xlsx) y `Vistas/` (B-V01, B-V02: XML + PNG) |
| `04_Phase_C_Data/` | `00_Comun_Fase_C/` (C-00 a C-06 y libro C3, comunes a datos y aplicaciones), `Catalogos_Matrices/` (C1) y `Vistas/` (D-V01..D-V03, genealogía) |
| `05_Phase_C_Application/` | `Catalogos_Matrices/` (C2) y `Vistas/` (AP-V01..AP-V03, X-V01) · ver `LEEME.md` |
| `06_Phase_D_Technology/` | T-00 a T-09, `Catalogos_Matrices/` (T1 v0.3, T2 v0.2) y `Vistas/` (T-V01..T-V10, X-V02: PNG + XML corregidos v0.2) |
| `07_Entregables_Integrados/` | `07-01` registros integrados B/C/D (Gap Register único, ARS, CRC, trazabilidad), `07-02` ADD/ARS consolidados, `Informe_PC3_Secciones/` |
| `08_ArchiMate_Modelos/` | Modelo integrado (XML + .archimate), `Vistas_SVG/`, `Vistas_PNG/`, `08-01` registro del modelo |
| `09_Evidencia_Fuentes/` | `09-01` dossier de evidencia HP, Anexo H, supuestos SV, plan de validación NV y registro de uso de IA |
| `10_Plantillas_TheOpenGroup/` | `10-01` índice plantilla oficial → archivo usado y aplicabilidad de artefactos C/D (M/S) |
| `11_Sustentacion/` | PPT de defensa (v0.3 corta) y `11-01` índice de evidencia de las dos cadenas E2E |
| `_historico/` | Versiones anteriores que se conservan para no borrar historia (C2 v0.1, T1 v0.1, T2 v0.1, B-07 matriz v0.1, XML originales de la Fase D) |

## Reglas del repositorio

- No se renombran IDs de PC1/PC2. Los cambios se registran en `CHANGELOG.md` y en `00-01 › Decision_Log`.
- Una versión vigente por artefacto; las anteriores van a `_historico/`.
- Toda afirmación se etiqueta HP, IA, SV, DE o NV (guía §1.3). Lo marcado `[confirmar]` o `[completar]` (celdas rojas en los xlsx) está pendiente de su owner.
- Las rutas de este README y del MANIFEST son relativas a esta carpeta raíz.
