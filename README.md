# Contador-con-Display-de-7-Segmentos
Este proyecto consiste en la implementación de un contador decimal básico que cicla los números del 0 al 9 con un intervalo de un segundo entre cada dígito.

Materiales Necesarios
1x Arduino Uno (o similar)

1x Display de 7 segmentos (Cátodo Común)

7x Resistencias de 220Ω

1x Protoboard

Cables tipo "Dupont"

Diagrama de Conexión

Para mantener el código simple, conectaremos los segmentos (A-G) a los pines digitales del 2 al 8 en orden alfabético.

a -> pin 2

b -> pin 3

c -> pin 4

d -> pin 5

e -> pin 6

f -> pin 7

g -> pin 8

GND -> GND (con resistencia)

Instrucciones de Ensamblaje

Inserta el display en la protoboard.

Identifica los pines del display (suelen ser 5 arriba y 5 abajo). El pin central de ambos lados suele ser el común (GND en este caso).

Conecta el pin común a la línea de tierra (GND) del Arduino usando una resistencia para proteger los LEDs.

Conecta cada uno de los pines correspondientes a los segmentos a, b, c, d, e, f, g a los pines digitales 2 al 8 del Arduino, respectivamente.

https://github.com/user-attachments/assets/bdd609fb-9462-4355-bb3a-cda1f577afb1

