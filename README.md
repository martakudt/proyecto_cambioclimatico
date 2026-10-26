# 🌍📊 Análisis Exploratorio de Datos: Cambio Climático

Proyecto de **Análisis Exploratorio de Datos (EDA)** desarrollado en el **Bootcamp de Data Science & IA de EDEM**.

El objetivo es aportar evidencia empírica sobre la existencia del cambio climático y su relación con la actividad humana, analizando la evolución de la temperatura global y de la concentración de CO₂ en la atmósfera, los principales países emisores de gases de efecto invernadero, el desplazamiento de icebergs como consecuencia visible y el auge del negacionismo climático en redes sociales.

---

## 📂 Estructura del repositorio

```
proyecto_cambioclimatico/
├── EDA.ipynb                            # Memoria del proyecto: contexto, resumen y conclusiones
├── 1.calentamiento_global.ipynb         # Emisiones de gases de efecto invernadero por país
├── 2.negacionismo_comentarios_x.ipynb   # Evolución de tuits negacionistas (2020-2022)
├── 3.temperatura_y_co2.ipynb            # Temperatura global vs. concentración de CO₂ (1983-2023)
├── 4.desplazamiento_icebergs.ipynb      # Trayectorias de icebergs en la Antártida
├── presentacion.pdf                     # Presentación del proyecto
├── data/                                # Datasets originales y procesados
├── img/                                 # Imágenes usadas en los notebooks
└── requirements.txt
```

> 💡 Si solo quieres una visión general, empieza por [EDA.ipynb](EDA.ipynb) o por la [presentación](presentacion.pdf).

---

## 📒 Notebooks

### 🌡 1. Calentamiento global — [1.calentamiento_global.ipynb](1.calentamiento_global.ipynb)
Emisiones totales de gases de efecto invernadero (millones de toneladas de CO₂ equivalente) por país entre 1983 y 2023, para identificar a los principales emisores.

### 🗣 2. Negacionismo en X — [2.negacionismo_comentarios_x.ipynb](2.negacionismo_comentarios_x.ipynb)
Evolución del número de tuits negacionistas sobre el cambio climático entre 2020 y 2022, a partir de los datos publicados en un artículo periodístico.

### 🌿 3. Temperatura global y niveles de CO₂ — [3.temperatura_y_co2.ipynb](3.temperatura_y_co2.ipynb)
Ambos análisis están en el mismo notebook para poder compararlos directamente en el periodo 1983-2023:
- Evolución anual, por décadas y por estaciones de las anomalías de temperatura (NASA GISTEMP).
- Evolución de la concentración de CO₂ atmosférico (NOAA).
- Correlación entre CO₂ y temperatura.
- Influencia de El Niño y La Niña en las fluctuaciones de temperatura.
- Comparación entre la media mensual de CO₂ (`average`) y la tendencia desestacionalizada (`trend`).

### 🧊 4. Desplazamiento de icebergs — [4.desplazamiento_icebergs.ipynb](4.desplazamiento_icebergs.ipynb)
Trayectorias de los icebergs con más observaciones y mapa interactivo (folium) de los icebergs más grandes.

---

## 📊 Principales conclusiones

- **Emisiones concentradas**: un grupo reducido de países (China, Estados Unidos, la Unión Europea, Rusia e India) acumula la mayor parte de las emisiones globales.
- **CO₂ y temperatura**: la correlación entre la concentración de CO₂ y la temperatura media anual es de **0.94**, una relación positiva muy fuerte que respalda el vínculo entre emisiones y calentamiento global.
- **Ciclo estacional del CO₂**: la mayor diferencia entre `average` y `trend` se da en abril y la menor en agosto-septiembre, reflejo de la actividad fotosintética de la vegetación del hemisferio norte.
- **El Niño y La Niña**: explican parte de las subidas y bajadas puntuales de temperatura, pero no alteran la tendencia de calentamiento a largo plazo.
- **Negacionismo**: los tuits negacionistas pasaron de unos 220.000 en 2020 a unos 850.000 en 2022, lo que puede reducir la presión social para aplicar políticas climáticas.
- **Icebergs**: el desprendimiento y desplazamiento de grandes masas de hielo es una de las consecuencias visibles del aumento de las temperaturas en los polos.

---

## 🗃 Fuentes de datos

| Tema | Fuente |
|------|--------|
| Emisiones de gases de efecto invernadero | [World Bank – Total greenhouse gas emissions (Mt CO₂e)](https://data.worldbank.org/indicator/EN.GHG.ALL.MT.CE.AR5) |
| Temperatura global | [NASA GISS Surface Temperature Analysis (GISTEMP v4)](https://data.giss.nasa.gov/gistemp/) |
| Concentración de CO₂ | [NOAA Global Monitoring Laboratory](https://gml.noaa.gov/ccgg/trends/) |
| Posiciones de icebergs | [Kaggle – Iceberg Locations](https://www.kaggle.com/datasets/joelhanson/iceberg-locations) |
| Tuits negacionistas | [Información – Twitter, refugio y altavoz de negacionistas (2023)](https://www.informacion.es/medio-ambiente/2023/01/16/convierte-twitter-refugio-altavoz-negacionistas-81239440.html) |

Lectura complementaria: [El País – Apóstoles del negacionismo](https://elpais.com/elpais/2019/09/18/eps/1568820907_023534.html)

---

## 🚀 Cómo ejecutarlo

Requisitos: Python 3.x

```bash
git clone https://github.com/martakudt/proyecto_cambioclimatico.git
cd proyecto_cambioclimatico
pip install -r requirements.txt
jupyter notebook
```

Abre cualquiera de los notebooks y ejecuta las celdas en orden. Los datos necesarios ya están en la carpeta `data/`.

---

## 🛠 Tecnologías

Python · pandas · NumPy · matplotlib · seaborn · SciPy · folium · Jupyter
