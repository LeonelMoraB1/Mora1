# 

El gpio_put ( IN1, 1 )
La entrada IN1 toma un valor de 1 

Es para controlar el motor

gpio_put(IN1, 1);----\
                                     Motor derecho
gpio_put(IN2, 0);----/
Cómo la entrada IN1 tiene un valor de 1 el motor va a girar haciendo que, si gira solo ese motor, el robot girara hacia la izquierda

gpio_put(IN3, 1);----\
                                   Motor izquierdo 
gpio_put(IN4, 0);----/
La entrada IN3, que da al motor izquierdo, tiene un valor de 1 el motor va a girar hacia adelante, si este es el único girando el robot va a girar a la derecha 
Tomando en cuenta los dos ejemplos anteriores, si las entradas IN1 e IN3 son positivas (o valor de 1)  el robot podrá avanzar 
Este código permite al robot retroceder 
gpio_put(IN1, 0); gpio_put(IN2, 1);    Motor derecho 
gpio_put(IN3, 0); gpio_put(IN4, 1);   Motor izquierdo 
Printf("Motores : Adelante (W)\n" );

Estos códigos están dentro de condiciones condicionales, cuando se quiera que el robot se mueva hacia adelante, se ejecutará el condicional para avanzar.
