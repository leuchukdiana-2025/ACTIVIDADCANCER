# ACTIVIDADCANCER
Clasificación de tumores de mama con KNN (usando 3 variables)

En el primer paso se cargó y se realizó la exploración del data.csv. Procediendo a revisarse la estructura con ‘df.head()’ y ‘df.info()’.
La variable ‘diagnosis’ se convirtió a valores binarios (B=0, M=1).
En un segundo paso se seleccionó las variables a utilizar, el escalado con ‘StandardScaler’ y la división en train/test. 
 
Se entrenó un modelo KNN con `k=5`, realizándose pruebas con valores manuales. 
Se evaluaron los siguientes casos:

radius_mean  texture_mean  smoothness_mean
      17.99         10.38          0.11840
      20.57         17.77          0.08474
      19.69         21.25          0.10960




Para finalizar se realizó el histograma de `radius_mean`, la matriz de correlación y el gráfico de dispersión (`radius_mean` vs `texture_mean`).  

Con solo 3 variables (‘radius_mean’, ‘texture_mean’, ‘smoothness_mean’), el modelo logra una buena precisión en la clasificación.  Las variables seleccionadas: ‘radius_mean’ y ‘texture_mean’ muestran diferencias notorias en las distribuciones entre tumores benignos y malignos, aportando gran valor predictivo.  


