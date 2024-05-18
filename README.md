# Understanding Career Aspirations of GenZ
## Descripción General
El proyecto consiste en un análisis exploratorio de datos (EDA) de una encuesta sobre las preferencias de trabajo de la Generación Z en la India.
Luego, se desarrolla un modelo de Aprendizaje Automático para predecir la probabilidad de que un individuo esté dispuesto a trabajar para un mismo empleador por más de tres años.
Se entrenó el modelo como una Red Neuronal, bajo el modelo de Arboles de Decisión.
El archivo **'Proyecto Final Modulo 7.ipynb'**, Notebook de Jupyter desarrollado en Google Colab, **contiene 3 secciones o etapas**. **1:** El EDA, que analiza el DataFrame que llamamos 'df' 
y al que le pasamos los datos 'aspirationsGenZ.csv' que obtuvimos de Kaggle (Enlace de los datos al final). **2:** Seguido y limpiando los datos, pasamos a llamar al DataFrame 'cleaned_df'
en el cual trabajamos la normalización de los datos y creamos la copia 'datos', para la implementación posterior del modelo que llamamos 'modelo_arbol' que usa **'DecisionTreeClassifier'**.
**3:** Finalmente después de entrenar el modelo examinar su precisión, ajustar hiperparametros para un mejor rendimiento, hacemos una sencilla API con Flask, para realizar solicitudes POST a la API implementando nuestro modelo.
Se aclara que por los pocos datos para analizar, entrenar e implementar nuestro modelo, a partir de 'aspirationsGenZ.csv', el modelo NO es muy preciso: Se examinó la posibilidad de haber
implementado Clustering con los algoritmos de K-means y DBSCAN, y no fue satisfactoría las respuestas, lo cual llevo a implementar esta Red Neuronal, y de acuerdo al analisis, con el
algoritmo de Arboles de Decisión.
## Proposito del Modelo
Por medio del algoritmo de árboles de decisión, examinar las respuestas a las preguntas (Las variables mas relevantes) **"What type of Manager would you work without looking into your watch ?"**,
**"Which type of learning environment that you are most likely to work in ?"**, **"Which of the below Employers would you work with."**, **"What is the most preferred working environment for you."**,
y **"Would you definitely pursue a Higher Education / Post Graduation outside of India ? If only you have to self sponsor it."** para predecir la probabilidad de que el encuestado,
miembro de la Generación Z, acepte trabajar de 3 años o más con el mismo empleador; esto en el contexto del país de la India, con los datos recolectados y examinados.
Así en nuestro algoritmo, la variable dependiente o que hemos buscado predecir es **How likely is that you will work for one employer for 3 years or more ?**
## Contenido
- `Proyecto Final Modulo 7.ipynb`: Notebook de Jupyter con el análisis exploratorio de datos, Red Neuronal con algoritmo DecisionTreeClassifier, y despligue básico de una API Flask de nuestro modelo.
- `aspirationsGenZ.csv`: El archivo con los datos sobre 'Understand the career aspirations of Generation Z folks of India' que tomamos de Kaggle.

## Uso

Para utilizar este proyecto, sigue estos pasos:

1. Copia los archivos de este repositorio en tu Drive de Google (con tu cuenta email@gmail.com) .
2. Abre el archivo Proyecto Final Modulo 7.ipynb
3. Ve a la línea: df = pd.read_csv('/content/drive/MyDrive/Ucamp Ciencias de Datos 2023/Modulo 7/aspirationsGenZ.csv') y cambié la ruta **/content/drive/MyDrive/Ucamp Ciencias de Datos 2023/Modulo 7/aspirationsGenZ.csv** por su ruta en la cual guardo los archivos en Drive.
4. Ejecute en orden, paso a paso cada modulo o celda
5. Realiza solicitudes POST a la API para obtener predicciones utilizando el modelo entrenado.

## Créditos

Este proyecto fue desarrollado por José Miguel Caicedo (https://github.com/MikHope) como parte del proceso de aprendizaje y prueba de Técnicas avanzadas para ciencia de datos y empleabilidad.

## Enlaces

- https://www.kaggle.com/datasets/kulturehire/understanding-career-aspirations-of-genz
- https://colab.research.google.com/drive/1UtGzOGEMOespANe1MKDZgVGmu9TBvIuk?usp=sharing#scrollTo=93s0hxyZmtSC
