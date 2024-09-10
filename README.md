# Análisis de Ventas de Casas en el Condado de King

Este repositorio contiene un análisis completo de las ventas de casas en el Condado de King, Estados Unidos, realizado en un solo archivo de Jupyter Notebook. El análisis incluye la importación de datos, manipulación, análisis exploratorio, desarrollo de modelos predictivos y su evaluación.

## Estructura del Proyecto

- **data/**: Contiene el archivo de datos utilizado para el análisis (`kc_house_data.csv`).
- **notebooks/**: Incluye el notebook de Jupyter con todos los ejercicios y análisis.
  - `king_county_housing_analysis.ipynb`: Notebook que cubre todos los módulos del análisis.
- **images/**: Almacena imágenes y visualizaciones generadas durante el análisis (si es necesario).
- **scripts/**: Contiene scripts adicionales o funciones personalizadas que pueden haber sido utilizadas (si es necesario).
- **README.md**: Este archivo que explica la estructura y el propósito del proyecto.

## Acerca del Proyecto

El objetivo de este proyecto es predecir el precio de las casas en el Condado de King utilizando diversas características como tamaño, ubicación y número de habitaciones. El análisis se realiza en un único notebook dividido en los siguientes módulos:

1. **Importación de Datos**: Carga del dataset y primera exploración de sus características.
2. **Manipulación de Datos**: Limpieza de datos, manejo de valores faltantes, y eliminación de columnas innecesarias.
3. **Análisis Exploratorio de Datos**: Visualización y análisis de la relación entre diferentes características y el precio de las casas.
4. **Desarrollo de Modelos**: Creación de modelos predictivos utilizando regresión lineal y pipelines.
5. **Evaluación y Refinamiento de Modelos**: Evaluación de los modelos creados y refinamiento para mejorar su precisión.

## Cómo Usar este Repositorio

### 1. Clonar el Repositorio

Primero, clona el repositorio en tu máquina local utilizando Git. Abre una terminal y ejecuta el siguiente comando:

```bash
git clone https://github.com/tu_usuario/king_county_housing_analysis.git
```
### 2. Navegar al Directorio del Proyecto
Después de clonar el repositorio, navega al directorio del proyecto:
```
bash
cd king_county_housing_analysis
```
### 3. Instalar las Dependencias
Asegúrate de tener instaladas todas las dependencias necesarias. Puedes instalarlas utilizando el archivo requirements.txt:
```
bash
pip install -r requirements.txt
```
Este comando instalará todas las librerías necesarias para ejecutar el análisis, como pandas, numpy, matplotlib, seaborn y scikit-learn.

### 4. Abrir el Notebook en Jupyter
Abre el notebook en Jupyter Notebook:
```
bash
jupyter notebook notebooks/king_county_housing_analysis.ipynb
```
Ejecuta las celdas en el notebook para seguir el análisis paso a paso.

### 5. Ejecutar los Notebooks
Si no tienes Jupyter Notebook instalado, puedes instalarlo utilizando:
```
bash
pip install jupyter
```
Luego, inicia Jupyter Notebook con el siguiente comando:
```
bash
jupyter notebook
```
Esto abrirá una interfaz web donde podrás navegar hasta el directorio notebooks/ y abrir el notebook para ver y ejecutar el código.

## Resultados del Proyecto

Aquí se presentan los resultados y visualizaciones obtenidos durante el análisis.

### 1. Visualización de Datos Iniciales

- **Primera vista del DataFrame**
  ![DataFrame](images/dataframe_head.png)

- **Resumen estadístico del DataFrame**
  ![Summary Statistics](images/describe_summary.png)

### 2. Manipulación de Datos

- **Conteo de valores únicos en la columna 'floors'**
  ![Floor Counts](images/floor_counts.png)

- **Boxplot para determinar los valores atípicos en relación a la vista al mar**
  ![Waterfront Boxplot](images/waterfront_boxplot.png)

- **Regplot para determinar la correlación entre 'sqft_above' y 'price'**
  ![SQFT Above vs Price](images/sqft_above_regplot.png)

### 3. Correlación de Características

- **Correlación de características numéricas con el precio**
  ![Correlation Matrix](images/correlation_matrix.png)

### 4. Modelos de Regresión

- **Regresión Lineal usando la característica 'long'**
  ![Linear Regression Long](images/linear_regression_long.png)

- **Regresión Lineal usando 'sqft_living'**
  ![Linear Regression SQFT Living](images/linear_regression_sqft_living.png)

- **Regresión Lineal con múltiples características**
  ![Multiple Features Regression](images/multiple_features_regression.png)

- **Pipeline con características polinómicas**
  ![Polynomial Pipeline](images/polynomial_pipeline.png)

### 5. Evaluación y Refinamiento de Modelos

- **Ridge Regression en datos de prueba**
  ![Ridge Regression](images/ridge_regression.png)

- **Ridge Regression con características polinómicas de segundo orden**
  ![Ridge Polynomial Regression](images/ridge_polynomial_regression.png)

## Contribuciones
Si deseas contribuir al proyecto, por favor abre un issue o un pull request con tus cambios o sugerencias.

## Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.
