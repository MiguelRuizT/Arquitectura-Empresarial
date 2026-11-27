# 08_ArchiMate_Modelos · LEEME

**Modelo integrado v0.3** del Grupo 03 (caso Beta): un solo modelo con las 20 vistas de las Fases B, C y D.

| Archivo | Para qué |
|---|---|
| `SI605_PC3_Grupo03_Beta_Modelo_Integrado_v0.3.xml` | ArchiMate **Open Exchange Format** (XML). Es el archivo de referencia. |
| `SI605_PC3_Grupo03_Beta_Modelo_Integrado_v0.3.archimate` | Formato nativo de **Archi**. Abrir con *File → Open*. |
| `Vistas_SVG/` | Las 20 vistas exportadas en SVG, generadas a partir del XML. |
| `Vistas_PNG/` | Las figuras PNG originales de cada bloque (pueden mostrar etiquetas anteriores a la unificación de IDs). |
| `08-01_Registro_Modelo_Integrado_v0.3.xlsx` | Inventario de vistas, unificación de IDs y correcciones aplicadas. |

## Cómo abrirlo en Archi

1. **Opción A (nativo):** *File → Open* y seleccionar el `.archimate`.
2. **Opción B (recomendada si la A falla):** *File → Import → Open Exchange XML Model…* y seleccionar el `.xml`. Luego *File → Save As* para regenerar el `.archimate` con tu versión de Archi.
3. Revisar *Validate Model* y, si todo está bien, exportar de nuevo las vistas a PNG/SVG desde Archi (*File → Export → View As Image*) para reemplazar las figuras.

## Reglas de identificadores

- Negocio: IDs de B-06 (`id-STK-xx`, `id-E1..E7`, `id-BSV0x`).
- Datos y aplicaciones: IDs de C1/C2 (`id-DO1..DO8`, `beta-c-e-AC-0x`, `beta-c-e-APP-xx`); son la **autoridad** para la Fase D.
- Tecnología: IDs de los XML de la Fase D (`tabb-0x`, `nt-xx`, `zt-0x`, `cd-xx`, …); las relaciones repetidas `r1..r11` se prefijaron con la vista (`tv02-r1`, …).
