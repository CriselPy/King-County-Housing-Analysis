# Análisis de Ventas de Casas en el Condado de King
[![Python](https://img.shields.io/badge/Python-v3.9-3572A5.svg)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-v6.4.5-DA5B0C.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/license-MIT-purple.svg)](https://github.com/CriselPy/King-County-Housing-Analysis/blob/main/LICENSE/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-6495ed.svg)](https://github.com/CriselPy/King-County-Housing-Analysis/issues)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Cristina_Ortega-blue?logo=linkedin&style=flat-square)](https://www.linkedin.com/in/cristina-ortega-451750275/)
[![GitHub](https://img.shields.io/badge/GitHub-CriselPy-pink?logo=github&style=flat-square)](https://github.com/CriselPy)
[![GitHub stars](https://img.shields.io/github/stars/CriselPy/King-County-Housing-Analysis?style=social&label=Stars)](https://github.com/CriselPy/King-County-Housing-Analysis/stargazers)
[![Issues](https://img.shields.io/github/issues/CriselPy/King-County-Housing-Analysis?style=flat-square&color=673ab7)](https://github.com/CriselPy/King-County-Housing-Analysis/issues)

Este repositorio contiene un análisis completo de las ventas de casas en el Condado de King, Estados Unidos, realizado en un solo archivo de Jupyter Notebook. El análisis incluye la importación de datos, manipulación, análisis exploratorio, desarrollo de modelos predictivos y su evaluación.

## 📋 Tabla de contenidos
- [Binder](#-binder)
- [Visión General del Proyecto](#-visión-general-del-proyecto)
- [Tecnologías Utilizadas](#-tecnologías-utilizadas)
- [Instalación](#-instalación)
- [Configuración de Datos](#-configuración-de-datos)
- [Módulos de Análisis](#-módulos-de-análisis)
  - [Importación de Datos](#importación-de-datos)
  - [Manipulación de Datos](#manipulación-de-datos)
  - [Análisis Exploratorio de Datos](#análisis-exploratorio-de-datos)
  - [Desarrollo de Modelos](#desarrollo-de-modelos)
  - [Evaluación y Refinamiento de Modelos](#evaluación-y-refinamiento-de-modelos)
- [Estructura de Archivos](#-estructura-de-archivos)
- [Resultados](#-resultados)
  - [Tipos de Datos](#tipos-de-datos)
  - [Resumen Estadístico](#resumen-estadístico)
  - [Valores Únicos de 'floors'](#valores-únicos-de-floors)
  - [Boxplot de Precios por Vista al Mar](#boxplot-de-precios-por-vista-al-mar)
  - [Correlación entre 'sqft_above' y Precio](#correlación-entre-sqft_above-y-precio)
  - [Regresión Lineal con 'sqft_living'](#regresión-lineal-con-sqft_living)
  - [Regresión con Múltiples Características](#regresión-con-múltiples-características)
  - [Pipeline con Transformación Polinómica](#pipeline-con-transformación-polinómica)
  - [Regresión Ridge](#regresión-ridge)
  - [Regresión Ridge con Transformación Polinómica](#regresión-ridge-con-transformación-polinómica)
- [Documentación](#-documentación)
- [Contribuciones](#-contribuciones)
- [Autor](#-autor)
- [Licencia](#-licencia)

## 📦 Binder

Puedes ejecutar este proyecto directamente en un entorno interactivo en [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/CriselPy/King-County-Housing-Analysis/main?filepath=king_county_housing_analysis.ipynb). Esto te permitirá interactuar con el notebook sin necesidad de instalar nada en tu máquina local.

## 📖 Visión General del Proyecto

El objetivo de este proyecto es predecir el precio de las casas en el Condado de King utilizando diversas características como tamaño, ubicación y número de habitaciones. El análisis se realiza en un único notebook dividido en los siguientes módulos:

1. **Importación de Datos**: Carga del dataset y primera exploración de sus características.
2. **Manipulación de Datos**: Limpieza de datos, manejo de valores faltantes, y eliminación de columnas innecesarias.
3. **Análisis Exploratorio de Datos**: Visualización y análisis de la relación entre diferentes características y el precio de las casas.
4. **Desarrollo de Modelos**: Creación de modelos predictivos utilizando regresión lineal y pipelines.
5. **Evaluación y Refinamiento de Modelos**: Evaluación de los modelos creados y refinamiento para mejorar su precisión.

## ⚙️ Instalación

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
[requirements.txt](https://github.com/CriselPy/King-County-Housing-Analysis/blob/main/requirements)

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
Si no tienes Jupyter Notebook instalado, puedes instalarlo y luego iniciarlo para abrir el notebook.

## 📋 Estructura del Proyecto

- `king_county_housing_analysis.ipynb`: Notebook que cubre todos los módulos del análisis.
- **images/**: Almacena imágenes y visualizaciones generadas durante el análisis (si es necesario).
- **requirements.txt**: Archivo que lista todas las dependencias necesarias para ejecutar el proyecto.
- **README.md**: Este archivo que explica la estructura y el propósito del proyecto.
- **License**
- **.gitignore**
## 📝 Resultados del Proyecto

Aquí se presentan los resultados y visualizaciones obtenidos durante el análisis.

### 1. Tipos de Datos de Cada Columna

- **Visualización de los tipos de datos en el DataFrame**:
  ![Tipos de Datos](images/Captura%20de%20pantalla%202024-09-10%2020124139.png)

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
  ![Ridge Polynomial Regression](images/Captura%20de%20pantalla%202024-09-10%20125713.png)

## 📚 Documentación

En este proyecto se han utilizado varias tecnologías y herramientas. A continuación, se proporciona documentación relevante para cada una de ellas:

- **Documentación de Pandas:** [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
- **Documentación de NumPy:** [NumPy Documentation](https://numpy.org/doc/stable/)
- **Documentación de Matplotlib:** [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
- **Documentación de Seaborn:** [Seaborn Documentation](https://seaborn.pydata.org/)
- **Documentación de Scikit-learn:** [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- **Documentación de Jupyter Notebook:** [Jupyter Documentation](https://jupyter.org/documentation)

Esta sección proporciona una visión general de las herramientas y tecnologías empleadas en el proyecto para facilitar su comprensión y uso. Si necesitas más detalles sobre alguna tecnología específica, consulta la documentación proporcionada o busca recursos adicionales en línea.

## 🤝 Contribuciones

Este proyecto es una solución personal a un ejercicio del curso de IBM "Técnicas Avanzadas de SQL". Dado que fue completado de forma individual, no se incluyen contribuciones externas. ¡Sin embargo, las contribuciones son bienvenidas!

Si tienes sugerencias para mejorar los ejercicios, encuentras errores en las consultas o procedimientos, o tienes ideas para agregar nuevas características, te animo a contribuir. Puedes hacerlo de las siguientes maneras:

- **Abrir un Issue:** Si encuentras un error o tienes una sugerencia, abre un [issue](https://github.com/CriselPy/King-County-Housing-Analysis/issues) para discutirlo.
- **Enviar un Pull Request:** Si has realizado mejoras en el código o has solucionado un problema, siéntete libre de enviar un pull request.
- **Compartir tus propias soluciones:** Si deseas compartir tus propias soluciones o enfoques para los ejercicios, puedes hacerlo en los comentarios del repositorio.

Agradezco cualquier retroalimentación constructiva que pueda ayudar a mejorar el contenido. Tus contribuciones serán reconocidas y apreciadas.

## ✍️ Autor

Este proyecto fue completado por 
# Crisel Nublo🪻.

## 📜 Licencia

Este proyecto está licenciado bajo la Licencia MIT - consulta el archivo [LICENSE](https://github.com/CriselPy/King-County-Housing-Analysis/blob/main/LICENSE) para más detalles.
