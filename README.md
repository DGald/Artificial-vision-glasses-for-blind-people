Este código es un programa de detección de semáforos que utiliza una cámara para identificar semáforos en tiempo real y determinar su color y distancia:

El código comienza importando varias bibliotecas necesarias para su funcionamiento. cv2 es para el procesamiento de imágenes, numpy para cálculos matemáticos,
pyttsx3 para la síntesis de voz, y picamera para interactuar con la cámara Raspberry Pi.
Se inicializa un motor de voz.
Se definen varias constantes que se utilizarán más adelante en el código, como el tamaño real del semáforo, la distancia conocida desde la cámara al semáforo, y
el tamaño del semáforo en la imagen a una distancia conocida.
Se definen dos funciones, una para calcular la distancia desde la cámara al semáforo basándose en su tamaño en la imagen, y otra para detectar el color del semáforo.
Esta función toma una imagen y un archivo de clasificador en cascada (un tipo de clasificador de objetos) como entrada, detecta los semáforos en la imagen, dibuja un rectángulo alrededor de ellos, 
detecta su color, calcula la distancia a ellos, y da una alerta si la distancia es igual a la distancia conocida.
Se inicializa la cámara Raspberry Pi con una resolución y velocidad de fotogramas específicas para mejorar el rendimiento.
Finalmente, el código entra en un bucle donde captura continuamente cuadros de la cámara, detecta los semáforos en cada cuadro utilizando la función definida anteriormente, y muestra el resultado.

This code is a traffic light detection program that uses a camera to identify traffic lights in real time and determine their color and distance:

The code begins by importing several libraries necessary for its operation. cv2 is for image processing, numpy for mathematical calculations, pyttsx3 for voice synthesis, 
and picamera to interact with the Raspberry Pi camera. A voice engine is initialized. Several constants are defined that will be used later in the code, such as the real size of the traffic light, 
the known distance from the camera to the traffic light, and the size of the traffic light in the image at a known distance. Two functions are defined, one to calculate the distance from the camera 
to the traffic light based on its size in the image, and another to detect the color of the traffic light. This function takes an image and a cascade classifier file (a type of object classifier) as 
input, detects the traffic lights in the image, draws a rectangle around them, detects their color, calculates the distance to them, and gives an alert if the distance is equal to the known distance. 
The Raspberry Pi camera is initialized with a specific resolution and frame rate to improve performance. Finally, the code enters a loop where it continuously captures frames from the camera, detects 
the traffic lights in each frame using the previously defined function, and displays the result.
