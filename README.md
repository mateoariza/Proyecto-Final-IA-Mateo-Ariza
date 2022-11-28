# Proyecto-Final-IA-Mateo-Ariza
Desarrollado por: Mateo Felipe Ariza Ordóñez

Video Youtube:  https://youtu.be/aEUJrihKYeI
Se tiene como objetivo la predicción de qué tan satisfechos (satisfecho o no satisfecho) se encuentran los usuarios con una aerolínea. El dataset se encuentra en https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction. Los datos de entrenamiento tienen una cantidad de 103904 muestras. Con las siguientes características:

•	"Gender"

•	"Customer Type"

•	"Age","Class"

•	"Inflight wifi service"

•	"Ease of Online booking"

•	"Gate location","Food and drink"

•	"Online boarding","Seat comfort"

•	"Inflight entertainment"

•	"On-board service","Leg room service"

•	"Baggage handling","Checkin service"

•	"Inflight service" 

-Y como etiquetas tiene:

•	"satisfaction"

Se realizó preprocesamiento de los datos, normalización y PCA. Se propuso usar Regresión Logística, Máquinas de Soporte Vectorial y Redes Neuronales. Por medio de GridSearch se iteró para encontrar los mejores parámetros para cada uno de los métodos. El método que tenga mejor Coeficiente de correlación de Mathews es el seleccionado para la solución del problema.
![image](https://user-images.githubusercontent.com/85539855/204172684-28578092-8ff1-4c6f-a432-d0ff54583d1c.png)
![image](https://user-images.githubusercontent.com/85539855/204172773-6356efcb-3a12-4570-bdde-d72993586a67.png)
![image](https://user-images.githubusercontent.com/85539855/204172787-f43e7b61-d673-4d1d-9df8-8b8b59d800d2.png)

Conclusiones:

Como el dataset tiene mas de 100000 datos, el GridSearch de las máquina de soporte vectorial puede tardar alrededor de 6 horas. Esto se debe a que también se tiene 3 hiperparámetros con distintos valores a iterar.

Tomando el Score del Coeficiente de Matthews las redes Neuronales tuvieron un mejor desempeño con los datos de validación, el mejor resultado para el Accuracy fue también Redes neuroanles, pero en el resultado de la ROC la regresión logística fue mejor. Sin embargo, los resultados obtenidos fueron muy cercanos, al contrario de SVM que tuvo unos resultados relativamente bajos (Coeficiente de Matthews = 0.4881...).
