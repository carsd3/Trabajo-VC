# Trabajo-VC

En este trabajo hemos querido desarrollar el proceso de detección de basura de un prototipo de robot reciclador. Para ello primeramente hemos montado un dataset con distintos objetos reciclables y los hemos 
dividido en cuatro clases: latas, cartón, botellas de vidrio y botellas de plástico. Seguidamente, hemos entrenado un modelo de yolov8 con dicho dataset y preparado una pequeña simulación del proceso de 
actuación del robot.

Para ello, primero que nada cogemos lo que una imagen cualquiera que respresenta un frame de la cámara del robot. Procesamos dicha imagen y detectamos los contornos de la misma, iteramos sobre los "blobs" 
delimitados por dichos contornos y escogemos el más grande, que representaría un objeto en el suelo. Una vez tengamos ese fragmento de la imagen delimitado, utilizaremos el modelo ya entrenado para intentar 
comprobar si es un objeto reciclable o no y se acaba la ejecución.

A continuación se encuentra el enlace al colab: https://colab.research.google.com/drive/19DovagzoB4QWNxuD9-m26M56QbzZ0h_l?usp=sharing
