Gabriel Troyo B97893
# Proyecto4
## Problema
El proyecto consiste en una primera parte la cual consiste en transformar una imagen a formato de bits para luego ser transferida como señal.
Una vez se tiene la señal enviada viene la siguiente parte del proyecto, a la cual se le tiene que agregar un ruido "ficticio" dado a que la señal en realidad no se ha enviado, pero se quiere trabajar como si la señal hubiera sido recibida.
En la siguiente parte del proyecto consiste en procesar la señal con ruido en bits para recrear la imagen enviada.
Luego se tiene una pequeña prueba de estacionaridad y ergodicidad para las señales Tx. Finalmente se tiene una densidad espectral de potencia para la señal modulada.
## Resultados
Para la primer parte, que consiste en la transmision e interpretacion de una imagen mediante una señal se tiene que se resolvió con una modulacion y demodulacion de 16-QAM.
Para esto, se modificó el código de BSKP en ciertos puntos clave como la funcion de modulacion, para que este codigo fuera de un BPSK a 16-QAM se tiene que cambiar la generacion de 1 señal a dos señales, y luego se tiene que evaluar los bits de 4 en 4 y no individualmente para generar dichas señales, tambien se cambia la generacion del ruido y la demodulacion para que trabajen con dos señales y en la demodulacion cada 4 bits.
La imagen se logró conseguir con gran satisfaccion.
Para la segunda parte se obtuvieron valores referentes a la estacionaridad y ergodicidad, en donde todas las pruebas menos la de los promedios se consiguieron satisfactoriamente. 
Para la densidad espectral de potencia se consiguieron valores satisfactorios dado a que se muestra una distribucion cercana a una gaussiana principalmente en los valores de frecuencias de 5KHz (donde la señal originalmente fue enviada)
## Comentario de los resultados
La imagen se logró conseguir con gran satisfaccion dado a que muy pocos errores surgieron gracias a la exactitud de los parametros en la demodulacion ,dado a que originalmente se habian elegido los valor de 0.8 y esta daba muchos errores (pero aun se lograba distinguir la imagen) luego los de 1.5 ya daban resultados aceptables, pero cuando se utilizó el valor de 2 se dieron los mejores resultados posibles para distinguir las señales con ruido.
En la segunda parte todas las pruebas para la estacionaridad se consiguieron probar satisfactoriamente con valores no exactamente iguales, pero si muy similares.
Para la ergodicidad nose consiguió probar satisfactoriamente esta propiedad a pesar que la señal si la cumple, esto se puede deber a errores ligeros en el código.
Finalmente, en el espectro de densidad de potencias se tiene que los mayores valores obtenidos fueron con un punto central en los 5KHZ de frecuencia, lo cual era lo esperado y lo ideal, sino en caso contrario se tendría un espectro de potencia el cual no es referente a uno similar de la señal enviada originalemente, lo cual puede mostrar muchos errores en la señal y tambien se puede deber al ruido del ambiente.

