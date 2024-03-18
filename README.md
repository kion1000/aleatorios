Readmy Sobre el Ejercicio Aleatorio con Debbuger.

El error en el código proporcionado radica en cómo se está generando el número aleatorio. La línea que contiene el error es:

num_aleat[i]=(int)Math.random()*100;

El problema esta en que el Int que se está aplicando a Math.random(), devuelve un valor de tipo double en el rango de 0 (inclusive) a 1 (exclusivo). Al hacer la operacion antes de multiplicar por 100, se está limitando el resultado a 0 o 1.

Para corregir este error, he movido los parentesis situandolos antes del math.ramdon y al final de la multiplicacion por 100. De esta manera, el resultado de la multiplicación (que estará en el rango de 0 a 100 aproximadamente) devolvera los numeros Solicitados.

Adjunto las imagen de Las variables y los breakpoint:


![Captura de pantalla 2024-03-18 a las 18 47 14](https://github.com/kion1000/aleatorios/assets/150617180/a1223e53-4329-497b-aefe-9e217abaa724)

![Captura de pantalla 2024-03-18 a las 18 47 45](https://github.com/kion1000/aleatorios/assets/150617180/48374d59-ae27-44c5-83e5-e26934f31ef4)


Adjunto imagen de el valor del iterados al ir pulsando Step Over:


![Captura de pantalla 2024-03-18 a las 18 48 04](https://github.com/kion1000/aleatorios/assets/150617180/f477ef1a-bbb6-47de-b1a1-6c57c51450ed)


![Captura de pantalla 2024-03-18 a las 18 48 21](https://github.com/kion1000/aleatorios/assets/150617180/da32a773-3114-481f-ad06-3434f78b7656)


Y por ultimo adjunto imagen de los números impresos en la consola:

![Captura de pantalla 2024-03-18 a las 18 48 45](https://github.com/kion1000/aleatorios/assets/150617180/0ab0e246-2a7f-4b20-a4b1-5a4f86a96658)

Aqui la linea corregida:

num_aleat[i] = (int)(Math.random() * 100);

He subido todo el proyecto con el archivo java.
