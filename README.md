<p align="center">
<img src="chunga-malaje-consulting.png" width="520">
</p>

# Brecha de género en empleo HRST en Europa

![Tableau](https://img.shields.io/badge/Tableau-Data%20Visualization-blue)
![Eurostat](https://img.shields.io/badge/Data-Eurostat-orange)
![EDA](https://img.shields.io/badge/Analysis-EDA-purple)
![Dashboard](https://img.shields.io/badge/Dashboard-Interactive-blueviolet)

Proyecto de análisis y visualización de datos desarrollado en **Tableau** a partir de datos públicos de **Eurostat** para estudiar la **brecha de género en el empleo en ciencia y tecnología (HRST)** en Europa.

Evaluación final del **Módulo 4 – Data Visualization**  
Bootcamp Data Analytics — **Adalab**

Autores:  
**Ruth Pérez Segovia**  
**Marina Martín Díaz**

---

# Objetivo del análisis

El objetivo de este proyecto es analizar la **brecha de género en el empleo HRST (Human Resources in Science and Technology)** en Europa y explorar cómo se distribuye en función de:

- el **sexo**
- la **evolución temporal**
- el **país**
- la **edad**

El análisis se materializa en un **dashboard interactivo** que permite explorar diferencias territoriales, tendencias temporales y patrones demográficos en el empleo científico-tecnológico.

---

# Preguntas analíticas

El dashboard está diseñado para responder tres preguntas principales:

**1️⃣ ¿Cómo evoluciona el empleo HRST por sexo a lo largo del tiempo?**

**2️⃣ ¿Qué países presentan mayor o menor brecha de género relativa?**

**3️⃣ ¿Cómo se distribuye el desempleo HRST según grupo de edad?**

---

# Dashboard final

El dashboard integra:

- KPIs principales
- evolución temporal del empleo HRST
- mapa temático por país
- ranking de brecha de género relativa
- distribución del desempleo por edad
- filtros interactivos

Elementos incluidos:

- **3 KPIs**
- **4 visualizaciones**
- **filtros interactivos**
- **interacciones entre gráficos**

---

# KPIs incluidos

El panel superior resume el estado general del fenómeno mediante tres indicadores:

- **% medio de mujeres en empleo HRST**
- **Brecha media relativa**
- **Número de países con datos disponibles**

Estos indicadores permiten contextualizar rápidamente el análisis antes de explorar las visualizaciones.

---

# Visualizaciones del dashboard

### Evolución del empleo HRST por sexo
Gráfico de líneas que muestra la evolución temporal de la presencia de mujeres y hombres en el empleo HRST.

Permite identificar tendencias y posibles convergencias o divergencias entre ambos grupos.

---

### Brecha relativa por país
Mapa temático que representa la brecha de género relativa en empleo HRST para cada país europeo.

Facilita detectar patrones geográficos y diferencias territoriales.

---

### Países con mayor y menor brecha
Ranking de países que muestra los extremos en la distribución de la brecha de género relativa.

Permite comparar rápidamente qué países presentan mayor desigualdad relativa.

---

### Desempleo HRST por edad
Gráfico de barras que muestra la distribución del desempleo en HRST por grupos de edad.

Introduce una dimensión demográfica que complementa el análisis de género.

---

# Interactividad

El dashboard incluye varios elementos interactivos:

**Filtros**

- año
- país

**Interacciones entre visualizaciones**

- selección en el mapa filtra el ranking
- selección en el mapa actualiza otras visualizaciones

Esto permite explorar el dataset de forma dinámica y descubrir patrones específicos.

---

# Fuentes de datos

Los datos proceden de **Eurostat**, utilizando tres datasets principales:

- `hrst_st_nsecsex2`  
  Empleo en ciencia y tecnología por categoría HRST, actividad económica y sexo.

- `hrst_st_nunesex`  
  Personas desempleadas en ciencia y tecnología por categoría y sexo.

- `hrst_st_nuneage`  
  Personas desempleadas en ciencia y tecnología por categoría y grupo de edad.

Los datos se descargaron en formato **TSV**.

---

# Preparación y transformación de datos

Durante el proceso de preparación se realizaron varias tareas:

- limpieza de valores nulos
- normalización de tipos de dato
- creación de campos calculados
- filtrado de agregados supranacionales
- normalización de nombres de países
- preparación de variables para visualización

Campos calculados destacados:

- porcentaje de mujeres
- brecha de género relativa
- número de países con dato
- filtro de países válidos
- Top/Bottom 10 de brecha

---

# Tecnologías utilizadas

- **Tableau Desktop Public Edition**
- **Eurostat datasets**
- **Git / GitHub**

---

# Estructura del repositorio
