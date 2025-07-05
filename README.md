# Práctica 1: Análisis de Datos de Ecobici CDMX
 # Integrantes:
 
Fernando Espejel Rebollar.
Emma Edith Martínez Méndez.
Lesli Berenice Marín Montes.
María Fernanda Pazarán Yáñez.
Guilllermo Armando Lopez Ayala.

# Resumen del Proyecto - Análisis de Datos de Ecobici CDMX
El objetivo de este proyecto es integrar, limpiar y analizar la base histórica de viajes de Ecobici de la Ciudad de México, comprendida entre los años 2010 y 2025. Se busca unificar los datos de múltiples archivos CSV en un solo DataFrame de gran tamaño (aproximadamente 120 a 140 millones de registros) utilizando Python y la librería Pandas.

Posteriormente, se realiza un proceso de transformación de variables, destacando el cálculo de la duración de los viajes y la clasificación de la edad de los usuarios en rangos. Finalmente, se generan visualizaciones gráficas para identificar patrones de uso, tendencias demográficas y comportamientos de los usuarios.

Los resultados permitirán comprender mejor el perfil de los usuarios de Ecobici y el uso del sistema, facilitando la toma de decisiones y el diseño de estrategias de movilidad sustentable en la ciudad

# Instrucciones para ejecutar el notebook en Google Colab
Abrir el notebook en Colab
Haz clic en el archivo .ipynb dentro del repositorio o abre Google Colab y selecciona Archivo > Abrir cuaderno > GitHub e ingresa la URL de este repositorio para cargar el notebook.

Descarga manual de datos
Debido a restricciones de acceso, los datos necesarios deben descargarse manualmente:

Dirígete a [https://colab.research.google.com/drive/1in0jdh0Ic8HpjNw4J4GCpKXEe3aBbYtq?usp=sharing] 

Descarga los archivos CSV (o el formato correspondiente) necesarios para el análisis.

Sube estos archivos al entorno de Colab usando la función de carga de archivos.

Subir los archivos de datos a Colab
Dentro del notebook, ejecuta la celda que contiene el siguiente código para cargar los archivos desde tu computadora:


Instalación de librerías necesarias
Antes de ejecutar el análisis, instala las librerías necesarias ejecutando la celda con:

import numpy as np
import pandas as pd
pd.set_option("display.max_rows", 1500)
import re
import matplotlib.pyplot as plt
import cufflinks as cf

Ejecutar el notebook
Ejecuta las celdas del notebook en orden para cargar los datos, procesarlos y generar los análisis y visualizaciones.

# Analisis y grafica de Genero usuario

![GRAFICA_A ](https://github.com/LICGUILLERMOMAC/PRACTICA-_1/blob/4aec58f607874541dfff91d8511b105222add2e4/grafica%20genero.png)





# Analisis y grafica de Barras de Edad de usuario.
![GRAFICA_A ](https://github.com/LICGUILLERMOMAC/PRACTICA-_1/blob/4aec58f607874541dfff91d8511b105222add2e4/grafica%20genero.png)








 # Analisis y grafica de Barras de bici   
![GRAFICA_A ](https://github.com/LICGUILLERMOMAC/PRACTICA-_1/blob/4aec58f607874541dfff91d8511b105222add2e4/grafica%20genero.png)

Barras de la variable de Género de los usuarios
Se puede observar que alrededor de 3.1 millones de registros son de género M (Masculino) y aproximadamente 1.25 millones de registros son de género F (Femenino), el número de usuarios identificados como M es más del doble que el de usuarios F, por lo cual se podría indicar una mayor participación de hombres en el servicio, o un sesgo en los datos recolectados.

Barras de las variables Edad y Edad_Rangos
Se observa una distribución sesgada a la derecha (asimétrica), donde las edades más comunes se encuentran entre los 20 y 40 años. Hay un pico claro entre los 25 y 35 años, dicho pico superior a 250,000 registros siendo las frecuencias más altas, lo que indica que la mayoría de los usuarios están en ese rango de edad, es decir, usado por adultos jóvenes y a partir de los 40 años, la frecuencia disminuye progresivamente, es la cola larga hacia edades mayores, se observa que hay usuarios registrados con edades superiores a los 70 e incluso más de 90 años, aunque en frecuencias muy bajas. Esto puede incluir tanto datos reales como posibles errores, ya que, hay registros con edades anómalas como 100.

En el caso de los rangos de edades, el dominante es 26-35, dicho grupo tiene la mayor frecuencia, con más de 2 millones de registros, se confirma que la mayoría de los usuarios del servicio son adultos jóvenes. La presencia decreciente en edades mayores (60+) es natural en servicios que implican movilidad física. La baja participación de menores de 18 podría deberse a requisitos de edad mínima o falta de independencia de transporte.

 # Analisis Gráficos de barras y pastel para variables discretas.
![GRAFICA_A ](https://github.com/LICGUILLERMOMAC/PRACTICA-_1/blob/4aec58f607874541dfff91d8511b105222add2e4/grafica%20genero.png)

 
Gráfico de pastel

Por género: el 71.2% de la población de XXXX registros, son de género M (Maculino) que hacen uso del servicio.
Por rango de edad: de una población de XXX, el 5.4% tienen la edad de 30 años, posteriormente con 5.2% y 5.1% las edades de 31 y 28, respectivamente.
Finalmente, podemos concluir que el género M es el que usa con mayor frecuencia el medio de transporte de bicileta, además que los adultos jóvenes que son los del rango de edad entre 25 a 35 años son los que mayormente hacen uso del servicio.

































