# Expediente académico T&G Global · Preliminary y Phase A

Proyecto TG-EA-OMA-2026. Los datos H del Anexo H son hechos de partida dentro del escenario de enseñanza. Su procedencia hipotética no debe atribuirse a fuentes públicas ni a decisiones corporativas reales.

Orden: Anexo H y fuentes, PRE-01 a PRE-06, A-01 a A-06, repositorio y Enterprise Continuum. Los documentos incluyen el Anexo H al final. El estado Draft indica la etapa de revisión de cada artefacto.


## Actualización v1.3 — Sesión 5 / Phase B
- Se conserva la continuidad de Preliminary + Phase A.
- Se incorpora y consolida Phase B – Business Architecture.
- Todos los artefactos tabulares del expediente y del Architecture Repository se almacenan en formato Excel (.xlsx); no se utilizan CSV.
- Se mantiene B-06 en formato XML de intercambio ArchiMate para edición/importación en Archi.
- El Anexo H registra los datos hipotéticos H-01 a H-22 utilizados como valores válidos del escenario académico.

## Actualización v2.0 — Sesión integrada de Phase C (30 octubre 2026)

**Cobertura:** Preliminary → Phase A (Architecture Vision) → Phase B (Business Architecture) → Phase C Data Architecture → Phase C Application Architecture. **Phase D no desarrollada.** Los archivos heredados de v1.3 se conservan; las nuevas carpetas 06 a 09 y las subcarpetas Phase_C del Architecture Repository amplían, no sustituyen, lo anterior.

El caso sigue siendo **T&G Global / manzana premium / Whakatū / único value stream Orchard→Harvest→Packhouse→Cold Chain→Export→Market**. No corresponde a Del Monte Fresh Division; ese fue un ejercicio práctico distinto. La Baseline de aplicaciones es una **hipótesis de aula** y no debe presentarse como inventario interno verificado de T&G.

### Inicio de lectura recomendado

1. `00_Control/Anexo_H_Datos_del_Caso.xlsx` (H-01..H-22 anteriores) y `00_Control/Anexo_H_Extension_PhaseC.md` (H-C23..H-C32 nuevos).
2. `05_Phase_B/B-01_Business_Architecture_Definition.docx` para recordar capacidades CAP-01..06, servicios BSV-01..03, brechas GAP-B y requisitos BR.
3. `06_Phase_C_Entregables_TOGAF/C-01_Architecture_Deliverables_Data_Application_v2.0.docx` para mapear los artefactos recomendados por The Open Group a archivos, vistas y matrices reales del caso.
4. `C-02_Architecture_Definition_Document_ADD_v2.0.docx` y `C-03_Architecture_Requirements_Specification_ARS_v2.0.docx` (ambos dentro de carpeta 06).
5. Los tres libros `.xlsx` de `08_Phase_C_Catalogos_Matrices/`: C1 Datos (16 pestañas), C2 Aplicaciones (16 pestañas), C3 Trazabilidad y gobierno (11 pestañas).
6. `07_Phase_C_Vistas_ArchiMate/TG_ADM_Preliminary_PhaseA_PhaseB_PhaseC_15Views_OpenExchange_v2.0.xml`, que integra los modelos de A (4 vistas), B (3), C (7) y añade un puente B↔C (1).
7. `C-04_Architecture_Roadmap_Candidates_PhaseC_v2.0.docx` y `C-06_Architecture_Building_Blocks_Candidatos_v2.0.docx` (candidatos: sin cartera ni soluciones aprobadas).

**Jerarquía documental de TOGAF:** ADD explica cualitativamente Baseline y Target; ARS exige propiedades de arquitectura medibles; los catálogos/matrices/vistas detallan los bloques y relaciones; Roadmap contiene candidatos para fases posteriores. Requisito de negocio `BR-*` ≠ requisito de arquitectura `AR-D*`/`AR-A*` ≠ requisito funcional de un software `RF-*`. El proyecto de este curso **no** es el curso de Ingeniería de Requisitos.

**Importar XML en Archi:** `File > Import > Open Group ArchiMate Model Exchange File` y seleccionar el XML integrado. No se debe abrir el `.xml` con `File > Open`, que espera archivo nativo `.archimate`. Mantener los XML originales en `Modelos_Fuente` permite comprobar cambios y trazabilidad.

**Estado:** todos los entregables C son borradores docentes sujetos a gate; las metas numéricas adicionales H-C27 son supuestos del ejercicio. La arquitectura propuesta aún no está implantada ni aprobada por T&G.
