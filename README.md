# Proyecto: NLP en Reseñas de Vinos

## Descripción

Este proyecto implementa un pipeline de procesamiento de lenguaje natural (NLP) sobre un conjunto de datos de reseñas de vinos (`winemag-data-130k-v2.csv`). El objetivo es limpiar, tokenizar y analizar la frecuencia de palabras (unigramas y bigramas) para extraer insights sobre el lenguaje usado en las descripciones.

## Características

- Lectura y exploración inicial de datos con **pandas**.
- Eliminación de **stopwords** (palabras vacías) en inglés.
- Limpieza de **puntuación** usando expresiones regulares (`re`).
- **Tokenización** de texto con **NLTK** (`word_tokenize`).
- **Stemming** usando el `PorterStemmer` de NLTK.
- **Lemmatización** usando el `WordNetLemmatizer` de NLTK.
- Aplanamiento de listas de tokens para crear un corpus unificado.
- Cálculo de **frecuencias** de unigramas y bigramas con `nltk.ngrams` y `pandas.Series.value_counts()`.

## Tecnologías

- **Python 3.10+**
- **pandas**
- **NLTK** (tokenize, stopwords, stem, lemmatizer)
- **re** (expresiones regulares)
- **Jupyter Notebook**

## Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/tu_repositorio.git
   cd tu_repositorio
   ```
2. Crea un entorno virtual e instala dependencias:
   ```bash
   python -m venv venv
   source venv/bin/activate  # En Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```
3. Descarga el dataset `winemag-data-130k-v2.csv` y colócalo en la raíz del proyecto.

## Uso

1. Abre el notebook (`wine.ipynb`) en Jupyter:
   ```bash
   jupyter notebook wine.ipynb
   ```
2. Ejecuta todas las celdas para procesar los datos y generar las estadísticas de n-gramas.

## Estructura de Archivos

```
├── wine.ipynb                 # Notebook con el pipeline de NLP
├── winemag-data-130k-v2.csv   # Dataset de reseñas de vinos
├── requirements.txt           # Dependencias del proyecto
└── README.md                  # Documentación del proyecto
```

## Licencia

Este proyecto está bajo la licencia MIT. Siéntete libre de usarlo y adaptarlo.

