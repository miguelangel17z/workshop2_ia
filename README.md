# Workshop 2 — Machine Learning & Deep Learning Aplicado
**Universidad EAFIT · Introducción a la Inteligencia Artificial (2026-01)**
 
**Equipo:** Miguel Angel Garcia Osorio · Juan Ignacio · Samuel Granados
 
---
 
## Descripción
 
Este repositorio contiene el desarrollo de dos problemas de aprendizaje supervisado, cada uno abordado con un enfoque distinto según la naturaleza de su variable objetivo.
 
---
 
## Estructura del proyecto
 
```
├── clasificacion.ipynb   # Problema 1 — Clasificación
├── regresion.ipynb       # Problema 2 — Regresión
└── README.md
```
 
---
 
## Problema 1 · Clasificación — Detección de Fatiga Muscular en Ciclismo
 
**Dataset:** [Muscle Fatigue Cycling](https://huggingface.co/datasets/YominE/Muscle_Fatigue_Cycling) · Hugging Face  
**Objetivo:** Clasificar ventanas de señal EMG como estado normal (0) o fatiga muscular (1).
 
Se registraron señales de electromiografía en 8 músculos de la pierna dominante durante sprints en bicicleta. A partir de ventanas de 1 segundo se extrajeron 7 características por músculo en los dominios del tiempo y la frecuencia (RMS, varianza, ZCR, MAV, potencia espectral, frecuencia media y frecuencia mediana).
 
**Modelos evaluados:** KNN · Decision Tree · Random Forest · Gradient Boosting · DNN  
 
---
 
## Problema 2 · Regresión — Estimación de Edad a partir de Imágenes Faciales
 
**Dataset:** [Faces Age Detection](https://www.kaggle.com/datasets/arashnic/faces-age-detection-dataset) · Kaggle  
**Objetivo:** Predecir la edad cronológica de un sujeto a partir de su fotografía facial.
 
La variable objetivo es un valor numérico continuo en el rango [0, 116] años, lo que define el problema como regresión.
 
---
 
## Requisitos
 
```bash
pip install datasets scikit-learn tensorflow pandas numpy matplotlib seaborn scipy kagglehub
```
 
> Para el notebook de regresión se requiere configurar las credenciales de Kaggle (`KAGGLE_USERNAME` y `KAGGLE_KEY`) antes de ejecutar la descarga del dataset.
