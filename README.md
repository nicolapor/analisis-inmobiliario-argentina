# Análisis del Mercado Inmobiliario en Argentina

Proyecto completo de Data Science aplicado al mercado inmobiliario argentino, 
usando datos reales de Properati. Incluye análisis exploratorio, limpieza de 
datos, feature engineering y modelos predictivos de precios.

## Objetivo
Predecir el precio de propiedades en Argentina (en USD) a partir de 
características como tipo de propiedad, ubicación y superficie.

##  Dataset
- **Fuente:** Properati Argentina
- **Registros originales:** 121,220 propiedades
- **Registros finales:** 67,072 propiedades (tras limpieza)
- **Variables:** Tipo de propiedad, zona, superficie, precio en USD

## Tecnologías
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost

##  Estructura del Proyecto
- 01_EDA.ipynb # Análisis Exploratorio de Datos
- 02_Limpieza_Profunda.ipynb # Limpieza y tratamiento de datos
- 03_Feature_Engineering.ipynb # Creación y transformación de variables
- 04_Modelo_ML.ipynb # Entrenamiento y evaluación de modelos

## Resultados

| Modelo | MAE | RMSE | R² |
|--------|-----|------|----|
| Regresión Lineal | USD 61,519 | USD 83,376 | 0.42 |
| Random Forest | USD 45,153 | USD 67,634 | 0.62 |
| XGBoost | USD 45,526 | USD 66,222 | 0.64 |

**Mejor modelo:** XGBoost con R² de 0.64

## Hallazgos Principales
- Los **metros cubiertos** son la variable más influyente en el precio (25%)
- El tipo de propiedad **apartamento** es el segundo factor más importante (18%)
- **Bs.As. G.B.A. Zona Norte** y **Capital Federal** son las zonas más caras
- Las casas tienen un precio promedio de USD 225,000 vs USD 140,000 de los apartamentos

## Mejoras Futuras
- Aplicar NLP a la columna `description` para extraer características adicionales
- Incorporar datos de número de habitaciones y antigüedad
- Probar modelos más avanzados como LightGBM o redes neuronales

## Autor
**Nicolás Olave Portilla**  
Ingeniero de Sistemas | Ingeniero Industrial  
[LinkedIn](https://linkedin.com/in/nicolas-olave-portilla) | 
[GitHub](https://github.com/nicolapor)