<p align="center">
  <img src="assets/chunga-malaje-consulting.png" alt="Chunga&Malaje Consulting" width="500"/>
</p>

# Brecha de género en empleo HRST en Europa  
### Chunga&Malaje Consulting  
**Professional_code_RUTH_MARINA**

Evaluación final del Módulo 4 — Tableau / Data Visualization

Realizada por **Ruth Pérez Segovia** y **Marina Martín Díaz**  
Bootcamp de Data Analytics — Adalab

Proyecto centrado en análisis, visualización e interactividad para estudiar la brecha de género en empleo HRST en Europa a partir de datos públicos de Eurostat.

---

## Badges
**Status:** Finished  
**Tool:** Tableau Public / Tableau Desktop Public Edition  
**Data source:** Eurostat  
**Last updated:** 2026

---

## Descripción

Este repositorio contiene la resolución del proyecto final del **Módulo 4** del Bootcamp de Data Analytics de Adalab, orientado al diseño de un dashboard interactivo en Tableau.

El proyecto analiza la **brecha de género en el empleo HRST (Human Resources in Science and Technology)** en Europa, combinando varias fuentes de datos extraídas de **Eurostat** para construir una visión temporal, territorial y demográfica del fenómeno.

Se han utilizado tres datasets principales:

- **hrst_st_nsecsex2**: empleo en ciencia y tecnología por categoría HRST, actividad económica (NACE) y sexo.
- **hrst_st_nunesex**: desempleo en ciencia y tecnología por categoría y sexo.
- **hrst_st_nuneage**: desempleo en ciencia y tecnología por categoría y edad.

El resultado final es un **dashboard interactivo** que permite analizar la evolución del empleo HRST por sexo, la distribución geográfica de la brecha de género relativa, los países con mejor y peor posición comparada y el comportamiento del desempleo HRST por grupos de edad.

---

## Objetivo del proyecto

El objetivo principal del proyecto ha sido estudiar la **brecha de género en el empleo HRST en Europa** a través de un dashboard visual e interactivo que permitiera responder, al menos, a estas preguntas de análisis:

1. **¿Cómo evoluciona la presencia de mujeres y hombres en el empleo HRST a lo largo del tiempo?**
2. **¿Qué países presentan mayor o menor brecha de género relativa?**
3. **¿Cómo se distribuye el desempleo HRST según el grupo de edad?**

Además, el proyecto busca demostrar un flujo de trabajo completo en Tableau: selección de fuentes, limpieza, creación de campos calculados, diseño visual, construcción de interactividad y elaboración de conclusiones orientadas a análisis de datos.

---

## Selección de datasets y criterio analítico

La primera fase del trabajo consistió en explorar diferentes datasets de Eurostat relacionados con empleo, ciencia y tecnología. Finalmente, se seleccionaron tres fuentes que permitían combinar:

- dimensión **temporal**
- dimensión **territorial**
- dimensión de **género**
- dimensión **demográfica** (edad)

Se descartaron otras tablas complementarias porque añadían complejidad sin mejorar de forma clara la capacidad explicativa del dashboard.

El criterio de selección fue priorizar un análisis **coherente, visualizable y defendible**, frente a la acumulación de muchas fuentes sin una narrativa clara.

---

## Preparación y limpieza de datos

Los datos descargados desde Eurostat requerían una fase previa de transformación antes de poder utilizarse en Tableau.

### Trabajo realizado:

- Separación de campos agregados en columnas interpretables.
- Renombrado de variables para hacerlas comprensibles.
- Limpieza de valores y creación del campo **Valor limpio**.
- Gestión de valores nulos.
- Revisión de tipos de datos.
- Exclusión de agregados supranacionales no comparables como `EU27_2020` o `EA21`.
- Normalización de nombres de país para mejorar filtros y visualización.

### Campos calculados principales

Se construyeron varios campos calculados clave para el análisis:

- **Porcentaje de mujeres**
- **Brecha de género relativa**
- **Número de países con dato**
- **Es país**
- **País visual**
- **País mapa**
- **TopBottom 10**

Estos cálculos permitieron transformar la información original en indicadores interpretables y comparables entre países y años.

---

## Estructura del análisis

### 1️⃣ Fase 1 — Exploración y limpieza
- Carga de los datasets de Eurostat.
- Revisión de dimensiones y medidas disponibles.
- Detección de valores nulos y campos no comparables.
- Creación de variables limpias y renombradas para Tableau.

### 2️⃣ Fase 2 — Construcción de métricas
- Diseño de indicadores de presencia femenina y brecha de género relativa.
- Recuento de países válidos con dato.
- Depuración de códigos de país y resolución de incidencias en mapas.

### 3️⃣ Fase 3 — Diseño de visualizaciones
Se construyeron varias visualizaciones y se descartaron algunas versiones intermedias hasta llegar a un dashboard final más claro y legible.

### 4️⃣ Fase 4 — Dashboard interactivo
Se diseñó un dashboard final con:
- KPIs principales
- evolución temporal
- comparación geográfica
- ranking de países
- distribución del desempleo HRST por edad
- filtro general e interacciones entre visualizaciones

---

## Visualizaciones incluidas en el dashboard

### KPIs
- **% medio de mujeres**
- **Brecha media**
- **Países con dato**

### Gráficos
- **Gráfico de líneas:** evolución del empleo HRST por sexo.
- **Mapa temático por países:** brecha relativa por país.
- **Ranking de barras:** países con mayor y menor brecha relativa.
- **Gráfico de barras:** desempleo HRST por grupo de edad.

---

## Interactividad

El dashboard incluye:

- **Filtro general de página por año**
- **Filtro por país**
- **Interacción funcional entre visualizaciones**

Ejemplos de interacción implementada:
- selección en el **ranking** para filtrar otras visualizaciones
- selección en el **mapa** para actualizar análisis relacionados

Esto convierte el dashboard en una herramienta no solo descriptiva, sino también exploratoria.

---

## Principales insights

Algunos de los hallazgos más relevantes del análisis son:

- La presencia media femenina en el empleo HRST se sitúa en torno al **49,6 %** en la configuración actual del dashboard.
- La **brecha media relativa** muestra un valor negativo, lo que indica una desigualdad persistente en el conjunto analizado.
- La distribución territorial de la brecha no es homogénea: algunos países presentan mejores resultados relativos que otros.
- El desempleo HRST presenta diferencias entre grupos de edad, lo que sugiere la conveniencia de incorporar una lectura demográfica al análisis de género.

---

## Recomendaciones

A partir del análisis realizado, proponemos:

- profundizar en el estudio de los países con mejores resultados relativos para detectar posibles buenas prácticas;
- incorporar en fases posteriores un análisis más detallado por sectores NACE;
- analizar conjuntamente la dimensión de género y la de edad en políticas de empleo y formación;
- seguir monitorizando la evolución temporal para identificar mejoras o retrocesos en la brecha.

---

## Tecnologías utilizadas

- **Tableau Public / Tableau Desktop Public Edition**
- **Eurostat** como fuente de datos principal
- **Git y GitHub** para control de versiones y entrega
- Trabajo complementario de limpieza, organización y documentación del proceso analítico

---

## Estructura del repositorio

```bash
├── data/
│   ├── estat_hrst_st_nsecsex2.tsv
│   ├── estat_hrst_st_nunesex.tsv
│   └── estat_hrst_st_nuneage.tsv
├── assets/
│   └── chunga-malaje-consulting.png
├── dashboard/
│   └── Brecha_genero_HRST_Europa_FINAL.twbx
├── docs/
│   └── informe_proyecto_modulo4.pdf
└── README.md
