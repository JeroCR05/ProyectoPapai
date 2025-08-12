# ProyectoPapai
Proyecto de análisis y predicción de zonas aptas para el cultivo de papa en Colombia usando árboles de decisión.

🌱 Proyecto PapaIA
Grupo: Jerónimo Cardona Rivillas, María Alejandra Quiroz Montoya, Joshua Olaya

📌 Descripción
El análisis considera variables como altitud y pH del suelo, basándose en datos obtenidos de estaciones meteorológicas y estudios de suelos.

El modelo clasifica cada región como Apta o No Apta y genera visualizaciones como gráficos, tablas y mapas interactivos.

📂 Contenido del repositorio
ProyectoPapaIA.ipynb → Notebook con todo el análisis y entrenamiento del modelo.

modelo_papa.pkl → Modelo de árbol de decisión entrenado.

dataset.csv → Dataset de entrada con nombres de municipios y coordenadas.

Informe PapaIA.docx → Informe con metodología, resultados y conclusiones.

Carpeta /imagenes → Gráficos y visualizaciones.

✅ Resultados principales
Precisión del modelo: 94%

Las zonas más aptas se concentran en la región Andina (Boyacá, Nariño, Cundinamarca, Antioquia).

Factores clave: altitud entre 2.500 y 3.200 msnm y pH entre 5.5 y 6.5.

📦 Requisitos
pip install pandas
pip install numpy
pip install geopandas
pip install rasterio
pip install matplotlib
pip install seaborn
pip install joblib
pip install folium
pip install shapely
pip install pyngrok
pip install colorama
pip install scikit-learn
pip install gradio
pip install streamlit

# Geoprocesamiento y datos espaciales
import rasterio
from shapely.geometry import Point
import folium
from folium.plugins import MarkerCluster
import geopandas as gpd  # Si en alguna parte trabajas con GeoDataFrames

# Visualización de datos
import matplotlib.pyplot as plt
import seaborn as sns

# Machine Learning y métricas
from sklearn.tree import DecisionTreeClassifier, plot_tree
from sklearn.model_selection import cross_val_score, train_test_split
from sklearn.metrics import classification_report, confusion_matrix
from sklearn.ensemble import RandomForestClassifier

# Utilidades
import joblib
import threading
import os

# Interfaz y conexión
import gradio as gr
from pyngrok import ngrok

# Colores en consola
from colorama import Fore, Style

