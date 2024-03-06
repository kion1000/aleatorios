Readmy Sobre el Ejercicio Aleatorio con Debbuger.

El error en el código proporcionado radica en cómo se está generando el número aleatorio. La línea que contiene el error es:

num_aleat[i]=(int)Math.random()*100;

El problema esta en que el Int que se está aplicando a Math.random(), devuelve un valor de tipo double en el rango de 0 (inclusive) a 1 (exclusivo). Al hacer la operacion antes de multiplicar por 100, se está limitando el resultado a 0 o 1.

Para corregir este error, debes mover el parentesis al final de la operación, después de haber multiplicado el número aleatorio por 100. De esta manera, el resultado de la multiplicación (que estará en el rango de 0 a 100 aproximadamente) devolvera los numeros Solicitados.

Aqui la linea corregida:

num_aleat[i] = (int)(Math.random() * 100);

He subido todo el proyecto con el archivo java.
