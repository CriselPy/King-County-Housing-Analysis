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
```bash
cd king_county_housing_analysis
```
### 3. Instalar las Dependencias
Asegúrate de tener instaladas todas las dependencias necesarias. Puedes instalarlas utilizando el archivo requirements.txt:
```bash
pip install -r requirements.txt
```
Este comando instalará todas las librerías necesarias para ejecutar el análisis, como pandas, numpy, matplotlib, seaborn y scikit-learn.

### 4. Abrir el Notebook en Jupyter
Abre el notebook en Jupyter Notebook:
```bash
jupyter notebook notebooks/king_county_housing_analysis.ipynb
```
Ejecuta las celdas en el notebook para seguir el análisis paso a paso.

### 5. Ejecutar los Notebooks
Si no tienes Jupyter Notebook instalado, puedes instalarlo utilizando:
```bash
pip install jupyter
```
Luego, inicia Jupyter Notebook con el siguiente comando:
```bash
jupyter notebook
```
Esto abrirá una interfaz web donde podrás navegar hasta el directorio notebooks/ y abrir el notebook para ver y ejecutar el código.

## Resultados del Proyecto

Aquí se presentan los resultados y visualizaciones obtenidos durante el análisis.

### 1. Tipos de Datos de Cada Columna

- **Visualización de los tipos de datos en el DataFrame**:
  ![Tipos de Datos](images/Captura%20de%20pantalla%202024-09-10%20124139.png)

### 2. Resumen Estadístico

- **Resumen estadístico del DataFrame después de eliminar las columnas 'id' y 'Sin nombre: 0'**:
  ![Resumen Estadístico](images/Captura%20de%20pantalla%202024-09-10%20124331.png)

### 3. Conteo de Valores Únicos de 'floors'

- **Conteo de valores únicos en la columna 'floors' convertido a DataFrame**:
  ![Conteo de Floors](images/Captura%20de%20pantalla%202024-09-10%20124827.png)

### 4. Boxplot de Precios por Vista al Mar

- **Boxplot que muestra la comparación de precios para casas con y sin vista al mar**:
  ![Boxplot Waterfront](images/Captura%20de%20pantalla%202024-09-10%20124904.png)

### 5. Correlación entre 'sqft_above' y Precio

- **Regplot mostrando la correlación entre 'sqft_above' y el precio**:
  ![Regplot SQFT Above](images/Captura%20de%20pantalla%202024-09-10%20124957.png)

### 6. Regresión Lineal Simple con 'sqft_living'

- **Modelo de regresión lineal usando 'sqft_living' y el valor R²**:
  ![Linear Regression SQFT Living](images/Captura%20de%20pantalla%202024-09-10%20125219.png)

### 7. Regresión Lineal con Múltiples Características

- **Modelo de regresión lineal usando múltiples características y el valor R²**:
  ![Multiple Features Regression](images/Captura%20de%20pantalla%202024-09-10%20125401.png)

### 8. Pipeline con Transformación Polinómica

- **Pipeline que incluye escalado de datos, transformación polinómica, y regresión lineal con su valor R²**:
  ![Polynomial Pipeline](images/Captura%20de%20pantalla%202024-09-10%20121146.png)

### 9. Regresión Ridge

- **Modelo de regresión Ridge ajustado con un parámetro de regularización de 0.1 y el valor R²**:
  ![Ridge Regression](images/Captura%20de%20pantalla%202024-09-10%20125534.png)

### 10. Regresión Ridge con Transformación Polinómica de Segundo Orden

- **Modelo de regresión Ridge utilizando una transformación polinómica de segundo orden con el valor R²**:
  ![Ridge Polynomial Regression](images/Captura%20de%20pantalla%202024-09-10%20121146.png)

## Contribuciones
Si deseas contribuir al proyecto, por favor abre un issue o un pull request con tus cambios o sugerencias.

## Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.
