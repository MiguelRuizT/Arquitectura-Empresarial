# Guía del repositorio T&G — hasta Phase C Application Architecture

**Alcance docente:** SI605 · 5.º ciclo · 30 de octubre de 2026. Es un caso académico hipotético, no un levantamiento de la arquitectura interna de T&G.

## 1. Qué quedó de las fases anteriores

- **Preliminary**: modelo organizacional de arquitectura, RACI, marco adaptado, principios, Request for Architecture Work y estructura del Architecture Repository.
- **Phase A**: visión de arquitectura, stakeholders, alcance, SoAW, borrador de ADD, escenario de negocio y vistas VIEW-01..04.
- **Phase B**: value stream Orchard→Harvest→Packhouse→Cold Chain→Export→Market; CAP-01..CAP-06, servicios BSV-01..03, GAP-B01..05, requisitos de negocio BR-01..05 y XML de tres vistas B-V01..03.
- **Phase C — Data**: Baseline/Target de datos, catálogo de objetos y componentes, diccionario y relaciones, matriz datos×etapas, calidad/seguridad/ciclo/migración, D-V01..03, seis GAP-D, seis AR-D y cuatro D-RC.
- **Phase C — Application**: cartera de componentes y servicios, siete interfaces, matrices aplicación×datos/funciones/roles/organización, vistas A-V01..03, seis GAP-A, seis AR-A y cuatro A-RC.
- **Integración**: X-V01 y X-V02, vista de resultados de negocio sustentados por datos y servicios de aplicaciones; ADD y ARS consolidados, ADR y riesgos.

## 2. Qué se entiende por artefacto

Un **catálogo** enumera building blocks y atributos; una **matriz** explicita relaciones o responsabilidades; una **vista** expresa un concern para un stakeholder (en una notación como ArchiMate). Una vista no es un informe entero ni el viewpoint es lo mismo que la vista: *viewpoint* define reglas y destinatarios; *view* es la representación concreta.

## 3. Archivo XML para abrir en Archi

1. Instalar y abrir Archi, compatible con importación **Open Group ArchiMate Model Exchange**.
2. Ir a `File > Import > Open Group ArchiMate Model Exchange File` (el texto exacto del menú puede variar con la versión).
3. Seleccionar `../07_Phase_C_Vistas_ArchiMate/TG_ADM_Preliminary_PhaseA_PhaseB_PhaseC_15Views_OpenExchange_v2.0.xml`.
4. Revisar el árbol de **Views** y ubicar las cuatro vistas de A, tres de B, siete de C y la vista agregada X-V02. Las IDs fueron prefijadas para evitar colisiones entre los modelos originales.
5. Si se desea comparar, importar por separado los XML `Modelos_Fuente/Original_A_*`, `Original_B_*` y `Original_C_*`; son instantáneas independientes y puede haber conceptos con nombres próximos.
6. Para almacenar el trabajo en formato nativo de Archi, después de importar, usar `Save As` y producir un archivo `.archimate`. **No** usar directamente `File > Open` sobre el `.xml`.

## 4. Ruta de revisión de C1

1. Leer `C-02` secciones de Baseline/Target Data y `D-V01` (códigos WMS/QA/ERP, todos hipotéticos).
2. Abrir pestaña `Entidades_Datos`: localizar `DOBJ-01 Lot`, `DOBJ-02 LotEvent`, `DOBJ-03 LotGenealogy` y `DOBJ-11 SourceMapping`.
3. Abrir `Relaciones_Logicas`: observar la relación 1:N entre lote y evento y el N:M resuelto mediante la entidad de genealogía. No confundir genealogía de fruta con lineage del registro.
4. En `Data_Owner`, `Calidad_Datos`, `Acceso_y_Proteccion`, identificar quién gobierna significado, quién opera el dato y quién puede tomar la decisión de liberación.
5. Seguir `Gaps_Datos` → `Requisitos_AR_D` → `Roadmap_D`. Identificar qué prueba y qué candidato responde a cada brecha.

## 5. Ruta de revisión de C2

1. Ubicar las fuentes Baseline `AP-01..04` y el componente de IoT `AP-05` marcado **no verificado**.
2. Distinguir `AP-06` componente, su servicio `LotHistory Query` y su interfaz `IF-03`; los tres no son sinónimos.
3. Examinar `Aplicacion_x_Dato`, `Comunicacion_Apps`, `Rol_x_App` y `Proceso_x_App`.
4. Verificar en X-V01 / X-V02 la relación con `BSV-01`, `BSV-02`, `BSV-03` y capacidades Phase B.
5. Seguir `Gaps_Apps` → `Requisitos_AR_A` → `Roadmap_A`; identificar dependencias D-RC→A-RC.

## 6. Preguntas para la sustentación

1. ¿Por qué `PK-0150`, `LOT-150-A` y `EXP-7781` **no** se pueden presumir equivalentes y qué evidencia falta?
2. ¿Qué diferencia hay entre `DOBJ-03 LotGenealogy` y el linaje de `D-V03`?
3. ¿Cuál es la diferencia exacta entre `BR-01`, `AR-D01`, `AR-A01` y un requisito funcional eventual de consulta por pantalla?
4. ¿Quién puede liberar el lote? ¿Una aplicación que sirve el historial o el rol de Calidad autorizado?
5. ¿Por qué D-RC01 precede a A-RC01/A-RC02 y qué comprobación habilita la siguiente ola?
6. ¿Qué queda **pendiente** para Phase D en vez de inventarse en Application Architecture?

## 7. Fuentes y límites

El contenido de TOGAF está adaptado desde las **plantillas originales v2.0 (julio de 2024)** que facilitó el docente. Como fuentes de referencia de arquitectura se usan The TOGAF Standard, 10th Edition, ArchiMate y el concepto de descripción de arquitectura de ISO/IEC/IEEE 42010. Ningún propietario, aplicación, sensor, interface o métrica del escenario debe atribuirse a un sistema real de T&G sin evidencia adicional.
