<h1 align="center"> Proyecto de Data Analytics — Análisis del Programa de Lealtad de Aerolínea</h1>

<p align="center">
    Bootcamp de Data Analytics & IA.
</p>

<p align="center">
  <img src="imageBootcamp.png" width="300">
</p>

---

## Índice de Contenidos

* [Resumen y Alcance del Proyecto](#resumen-y-alcance-del-proyecto)
* [Competencias Adquiridas (Objetivos)](#competencias-adquiridas-objetivos)
* [Análisis de Datos (Fase 1: Exploración y Limpieza)](#análisis-de-datos-fase-1-exploración-y-limpieza)
* [Análisis Estadístico y Visualización (Fases 2 y 3)](#análisis-estadístico-y-visualización-fases-2-y-3)
* [Evaluación de Diferencias (Fase 4)](#evaluación-de-diferencias-fase-4)
* [Herramientas](#herramientas)
* [Ejecución](#ejecucion)
* [Autoría](#autoría)

---

## Resumen y alcance del proyecto

Este repositorio contiene la resolución de la **Evaluación Final del Módulo 3** (Transformación y Análisis de Datos) del Bootcamp de Data Analytics de Adalab.

El proyecto se centra en el comportamiento de los clientes dentro de un programa de fidelización de una aerolínea. El ciclo de trabajo incluye la consolidación de fuentes de datos mediante **Pandas**, la limpieza de valores nulos, el análisis estadístico descriptivo y la creación de visualizaciones para comunicar hallazgos de negocio.

## Competencias Adquiridas Objetivos

* Consolidar datasets mediante la técnica de **Merge** en Pandas.
* Implementar estrategias de limpieza y **tratamiento de nulos** (imputación por mediana).
* Dominar el **Análisis Exploratorio de Datos (EDA)**.
* Crear visualizaciones avanzadas con **Matplotlib** y **Seaborn**.
* Realizar comparaciones estadísticas entre grupos (Educación vs. Reservas).
* Traducir métricas técnicas a interpretaciones de negocio en lenguaje natural.

## Análisis de datos fase 1 exploración y limpieza

Se trabajó con los archivos `Customer Flight Activity.csv` y `Customer Loyalty History.csv` siguiendo este flujo:

### 🔹 Fase 1 — Unión y Transformación de datos

* Se realizó un **Left Merge** utilizando la columna común `Loyalty Number`.
* Se analizaron 405,624 registros de actividad mensual cruzados con perfiles de clientes únicos.

### Limpieza e Imputación

* Se detectaron **4,238 valores nulos** en la columna `Salary`.
* **Tratamiento:** Se realizó una imputación utilizando la **mediana** para no sesgar los datos por valores atípicos.
* Se normalizaron las columnas de fecha y se verificó la integridad de los registros de cancelación.

## Análisis Estadístico y Visualización 
### 🔹 Fases 2 y 3
Se obtuvieron los siguientes *insights* fundamentales mediante el análisis descriptivo y visual:

| Pregunta de Negocio | Gráfico Utilizado | Hallazgo Clave |
| :--- | :--- | :--- |
| **Estacionalidad** | Line/Bar Plot | Incremento de reservas en **julio** y **diciembre**. |
| **Relación Distancia/Puntos** | Scatter Plot | Correlación perfecta (**1.0**); sistema de puntos proporcional. |
| **Ubicación** | Count Plot | El mercado principal se encuentra en **Ontario** y **British Columbia**. |
| **Brecha Educativa** | Boxplot | Los perfiles con **Doctor** y **Master** tienen los promedios salariales más altos. |
| **Segmentación** | Clustered Bar | Análisis de distribución por género y estado civil de los clientes. |

## Evaluación de Diferencias
### 🔹 Fase 4 

Se evaluó si existían diferencias significativas en el número de vuelos reservados según el nivel educativo.

* **Filtros:** Se aislaron las variables `Flights Booked` y `Education`.
* **Resultado:** Tras agrupar y calcular medias y desviaciones estándar, se determinó que **el nivel educativo no es un factor determinante** para la frecuencia de reserva, a pesar de las diferencias en el nivel de ingresos.

---

## Herramientas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" width="55" height="55"/>
  &nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" alt="Pandas" width="55" height="55"/>
  &nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="NumPy" width="55" height="55"/>
  &nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original.svg" alt="Jupyter" width="55" height="55"/>
  &nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" width="55" height="55"/>
</p>

* **Python:** Lenguaje base para el procesamiento de datos.
* **Librerías:** `Pandas`, `NumPy`, `Seaborn`, `Matplotlib`.
* **Visualización:** Gráficos estadísticos y exploratorios.
* **Entorno:** Jupyter Notebook en VS Code.

---

## Ejecucion

Para replicar el entorno de trabajo:

1.  **Clonar el repositorio:**
    ```bash
    git clone https://github.com/Adalab/bda-modulo-3-evaluacion-final-TamDb22.git
    ```
2.  **Instalar dependencias:**
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  **Ejecutar el Notebook de Python** (`evaluacion_final.ipynb`):
    * El script realiza la carga de los CSV, ejecuta la limpieza y genera los gráficos automáticamente.
    * Cada visualización incluye una interpretación detallada de los resultados.

---

Proyecto desarrollado por: 
<p align="center">
  <a href="https://github.com/TuUsuarioDeGitHub">
    <img src="https://github.com/TamDb22.png" width="80" height="80" style="border-radius:50%;" alt="Tu Nombre"/>
  </a>
</p>
<p align="center"><strong>✨ ¡Aprender es construir! ✨</strong></p>
