# Cuestionario de Evaluación: Comunicación por Sockets 📝

**Nombre del Estudiante:** Javier Romero 
**Fecha:** 25/03/2026

*Instrucciones: Responde a las siguientes preguntas basándote en la teoría de redes y en el análisis del código de nuestro proyecto. Sube este archivo con tus respuestas a tu repositorio como evidencia de trabajo.*

1. **¿Qué es una Dirección IP y para qué sirve en nuestro proyecto?**
   > Es el identificador que tiene cada dispositivo que nos y permitirá el poder conectar el dispositivo ESP32

2. **¿Qué es un Puerto de red? (Menciona qué puerto estamos usando en el código de la ESP32).**
   > Usamos el puerto 80 y es el numero que identifica el servicio

3. **Define con tus propias palabras qué es un Servidor en informática.**
   > Es el programa que envia datos a diversos equipos y que esta a la espera de señales

4. **¿Cuál es la diferencia entre un "Servidor" (Hardware/Software) y un "Servicio" (Service)?**
   > Un servidor es quien ejecuta el sistema y el servicio es la función que se llega a realizar
5. **Investigación: ¿Cuál es la diferencia técnica entre un "Socket TCP" normal y un "WebSocket"?**
   > Webosocket ayuda ala comunicación en tiempo real sobre la web y TCP 

6. **Analizando nuestro código: ¿Quién actúa como Servidor y quién actúa como Cliente? (Justifica tu respuesta mencionando qué funciones del código lo demuestran, ej. `bind()`, `connect()`).**
   > ESP32 es el servidor y el cliente el dispositivo porque utilizamos conectar y para realizr la conexión

7. **En el código de la computadora (Python), importamos la librería `threading` (Hilos). ¿Qué pasaría con la ventana de Tkinter si no usáramos hilos para recibir los datos de la red?**
   > Probablemente se quedaría estático ya que no posee los datos de la red y se encuentra en espera de los mismos para poder funcionar 

8. **¿Por qué es necesario usar bloques `try...except` cuando trabajamos con conexiones de red e Internet?**
   >  Para ver los posibles errores en nuestra conexión y que el programa no se llegue a cerrar

9. **En la función de encender el LED en Python, enviamos el comando así: `sock.send(b'ON')`. ¿Qué significa esa letra `b` antes de las comillas y por qué no enviamos un texto normal?**
   > Se envian los bytes por que los sockets utilizan datos binarios

10. **Describe brevemente el flujo de datos: ¿Qué camino recorre la información desde que giras el potenciómetro físicamente hasta que la barra se mueve en la pantalla de la computadora?**
    > El potenciometro envia un valor a ESP32 mandandolo por via red mediante sockets, para que lo pueda recibir la computadora y que se pueda actualizar la barra en Tkinter
