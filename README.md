# CDS Box-Jenkins Colombia

Modelación Box-Jenkins de los Credit Default Swaps (CDS) soberanos de Colombia mediante modelos ARIMA implementados en Python.

**Universidad Nacional de Colombia**
**Econometría II – 2026**

---

## Objetivo

Analizar la dinámica temporal de los CDS soberanos de Colombia mediante la metodología Box-Jenkins, identificando un modelo ARIMA parsimonioso capaz de describir adecuadamente el comportamiento de la serie y generar pronósticos de corto plazo.

---

## Estructura del repositorio

```text
cds-box-jenkins-colombia/
│
├── data/
│   ├── raw/
│   │   └── datos_poster.xlsx
│   └── processed/
│
├── notebooks/
│   └── 01_exploración_cds.ipynb
│
├── outputs/
│   ├── figures/
│   └── tables/
│
├── poster/
│
├── scripts/
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Datos

La base de datos utilizada corresponde a la serie histórica de los Credit Default Swaps (CDS) soberanos de Colombia y se encuentra almacenada en:

```text
data/raw/datos_poster.xlsx
```

---

## Metodología

El proyecto sigue la metodología Box-Jenkins para modelación de series de tiempo:

1. Exploración gráfica de la serie.
2. Evaluación de estacionariedad mediante pruebas ADF, PP y KPSS.
3. Transformación y diferenciación de la serie cuando es necesario.
4. Identificación preliminar mediante FAC y FACP.
5. Estimación de modelos ARIMA candidatos.
6. Selección de modelos utilizando criterios AIC y BIC.
7. Diagnóstico de residuos.
8. Generación de pronósticos e intervalos de confianza.

---

## Resultados principales

Se estimaron distintos modelos ARIMA sobre la serie de CDS colombianos y sobre sus transformaciones logarítmicas y diferenciadas. La selección final se realizó con base en criterios de parsimonia, significancia estadística de parámetros y diagnóstico residual.

Los resultados obtenidos sugieren que modelos de baja dimensión capturan adecuadamente la dinámica de corto plazo de la serie, permitiendo construir pronósticos e intervalos de confianza consistentes con la metodología Box-Jenkins.

---

## Reproducibilidad

### 1. Clonar el repositorio

```bash
git clone https://github.com/Satoshi-Stardust/cds-box-jenkins-colombia.git
```

### 2. Ingresar al proyecto

```bash
cd cds-box-jenkins-colombia
```

### 3. Instalar dependencias

```bash
pip install -r requirements.txt
```

### 4. Ejecutar el notebook principal

Abrir:

```text
notebooks/01_exploración_cds.ipynb
```

y ejecutar todas las celdas.

---

## Tecnologías utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* SciPy
* Statsmodels
* OpenPyXL
* Jupyter Notebook
* Git
* GitHub

---

## Equipo de trabajo

* Diego Pachón
* Jonnathan Peña
* Fernando Rodríguez

---

## Contexto académico

Repositorio desarrollado como proyecto académico para la asignatura **Econometría II** de la **Universidad Nacional de Colombia**, aplicando herramientas de análisis de series de tiempo y modelación ARIMA al estudio de los CDS soberanos colombianos.
