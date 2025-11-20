# Machine Learning Projects

Repositorio que agrupa varios proyectos de aprendizaje automático realizados con Python y scikit-learn. Cada notebook aborda un problema distinto empleando técnicas de exploración, transformación de datos, modelado y evaluación.

Actualmente incluye:

- `costesMedicos.ipynb`: Predicción de los costes de seguros médicos (variable `charges`) a partir de características demográficas y de estilo de vida.
- `literatura.ipynb`: Clasificación cronológica de fragmentos literarios para identificar el siglo (XVI–XX) del autor a partir del vocabulario.

---

## Tabla de Contenidos

1. [Requisitos y Entorno](#requisitos-y-entorno)
2. [Estructura del Repositorio](#estructura-del-repositorio)
3. [Proyecto 1: Predicción de Costes Médicos](#proyecto-1-predicción-de-costes-médicos)
4. [Proyecto 2: Evolución de la Literatura](#proyecto-2-evolución-de-la-literatura)
5. [Buenas Prácticas y Reproducibilidad](#buenas-prácticas-y-reproducibilidad)
6. [Posibles Extensiones](#posibles-extensiones)
7. [Licencia y Créditos](#licencia-y-créditos)

---

## Requisitos y Entorno

### Lenguaje y Librerías Principales
- Python 
- scikit-learn
- numpy / pandas
- matplotlib / seaborn
- statsmodels
- Biblioteca externa `apafib` (usada para cargar los datasets)

## Estructura del Repositorio

```
machine_learning_projects/
├── costesMedicos.ipynb     # Notebook de regresión (costes de seguros médicos)
├── literatura.ipynb        # Notebook de clasificación (fragmentos literarios por siglo)
├── README.md               
```

---

## Proyecto 1: Predicción de Costes Médicos

Notebook: `costesMedicos.ipynb`

### Objetivo
Predecir el coste del seguro médico (`charges`) a partir de atributos como edad, índice de masa corporal, número de hijos, sexo, tabaquismo y región.

### Dataset
Se carga mediante `load_medical_costs` de la librería `apafib`. Es una versión del dataset público disponible en Kaggle: Insurance (mirichoi0218).

### Apartados Abordados
- Exploración, Partición y PCA
- Regresión Lineal (scikit-learn) y Análisis de Residuos
-  Ampliación con Polinomios (grado 2)
- Regularización LASSO

## Proyecto 2: Evolución de la Literatura

Notebook: `literatura.ipynb`

### Objetivo
Clasificar fragmentos de texto según el siglo del autor (XVI al XX) usando representaciones del vocabulario y distintos modelos de clasificación.

### Dataset
Cargado con `load_literature` de `apafib`, retornando:
- Lista de textos.
- Lista de etiquetas (siglos o autores).
Fuente textual: Proyecto Gutenberg (fragmentos de 23 autores).

### Apartados Abordados

- Generación de Matrices de Características
- Visualización con t-SNE
- Naïve Bayes (Modelos Generativos)
- Regresión Logística (Modelo Discriminativo)
- Resultados Esperados (Indicativos)
- Elección de Modelo




## Licencia y Créditos

- Datos médicos: Adaptado del conjunto [Insurance (Kaggle)](https://www.kaggle.com/datasets/mirichoi0218/insurance).
- Textos literarios: Fragmentos del [Project Gutenberg](https://www.gutenberg.org/).


