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

Código del Proyecto (C++)
Este código utiliza una matriz bidimensional para definir qué segmentos deben encenderse para formar cada número.

//Contador 0-9 con Display de 7 Segmentos
//Leonardo Payan Lara

int a = 2;
int b = 3;
int c = 4;
int d = 5;
int e = 6;
int f = 7;
int g = 8;

void setup() {
  pinMode(a, OUTPUT);
  pinMode(b, OUTPUT);
  pinMode(c, OUTPUT);
  pinMode(d, OUTPUT);
  pinMode(e, OUTPUT);
  pinMode(f, OUTPUT);
  pinMode(g, OUTPUT);
}

void loop() {
  //0
  digitalWrite(a, HIGH);
  digitalWrite(b, HIGH);
  digitalWrite(c, HIGH);
  digitalWrite(d, HIGH);
  digitalWrite(e, HIGH);
  digitalWrite(f, HIGH);
  digitalWrite(g, LOW);
  delay(1000);

  //1
  digitalWrite(a, LOW);
  digitalWrite(b, HIGH);
  digitalWrite(c, HIGH);
  digitalWrite(d, LOW);
  digitalWrite(e, LOW);
  digitalWrite(f, LOW);
  digitalWrite(g, LOW);
  delay(1000);

  //2
  digitalWrite(a, HIGH);
  digitalWrite(b, HIGH);
  digitalWrite(c, LOW);
  digitalWrite(d, HIGH);
  digitalWrite(e, HIGH);
  digitalWrite(f, LOW);
  digitalWrite(g, HIGH);
  delay(1000);

  //3
  digitalWrite(a, HIGH);
  digitalWrite(b, HIGH);
  digitalWrite(c, HIGH);
  digitalWrite(d, HIGH);
  digitalWrite(e, LOW);
  digitalWrite(f, LOW);
  digitalWrite(g, HIGH);
  delay(1000);

  //4
  digitalWrite(a, LOW);
  digitalWrite(b, HIGH);
  digitalWrite(c, HIGH);
  digitalWrite(d, LOW);
  digitalWrite(e, LOW);
  digitalWrite(f, HIGH);
  digitalWrite(g, HIGH);
  delay(1000);

  //5
  digitalWrite(a, HIGH);
  digitalWrite(b, LOW);
  digitalWrite(c, HIGH);
  digitalWrite(d, HIGH);
  digitalWrite(e, LOW);
  digitalWrite(f, HIGH);
  digitalWrite(g, HIGH);
  delay(1000);

  //6
  digitalWrite(a, HIGH);
  digitalWrite(b, LOW);
  digitalWrite(c, HIGH);
  digitalWrite(d, HIGH);
  digitalWrite(e, HIGH);
  digitalWrite(f, HIGH);
  digitalWrite(g, HIGH);
  delay(1000);

  //7
  digitalWrite(a, HIGH);
  digitalWrite(b, HIGH);
  digitalWrite(c, HIGH);
  digitalWrite(d, LOW);
  digitalWrite(e, LOW);
  digitalWrite(f, LOW);
  digitalWrite(g, LOW);
  delay(1000);

  //8
  digitalWrite(a, HIGH);
  digitalWrite(b, HIGH);
  digitalWrite(c, HIGH);
  digitalWrite(d, HIGH);
  digitalWrite(e, HIGH);
  digitalWrite(f, HIGH);
  digitalWrite(g, HIGH);
  delay(1000);

  //9
  digitalWrite(a, HIGH);
  digitalWrite(b, HIGH);
  digitalWrite(c, HIGH);
  digitalWrite(d, LOW);
  digitalWrite(e, LOW);
  digitalWrite(f, HIGH);
  digitalWrite(g, HIGH);
  delay(1000);
}

https://github.com/user-attachments/assets/bdd609fb-9462-4355-bb3a-cda1f577afb1

