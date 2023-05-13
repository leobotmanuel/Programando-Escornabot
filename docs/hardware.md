La placa de control del robot [Escornabot](https://escornabot.com) se denomina [EscornaCPU](https://github.com/escornabot/electronics/tree/master/EscornaCPU/2.x) y la última versión es la 2.x.

En el esquema de la [versión 2.12](https://github.com/escornabot/electronics/blob/master/EscornaCPU/2.x/2.12/Escorna_CPU_2_12_ESQ.pdf) se ve los diferentes bloques.

<center>
![CPU_2_12](img/hardware/esquemaCPU_2_12.png)

CPU v.2.12
</center>

#**Teclado**
El esquema correspondiente al bloque del teclado.

<center>
![teclado](img/hardware/teclado.png)

Teclado
</center>
Observando el esquema del teclado hay un cable etiquetado con **A7** que va al microcontrolador (entrada analógica).

El funcionamiento del teclado es un **divisor de tensión**, la pulsación de cada una de las teclas va a dar un valor de tensión en función del número de resistencias en serie que haya. El valor correspondiente a cada tecla se puede obtener con el siguiente programa.

<center>
![progTeclado](img/hardware/progTeclado.png)

Programa valor teclado
</center>

#**Motores paso a paso**
Los motores del robot son del tipo paso a paso y para el control de la seuencia de pasos utiliza 4 pines digitales.

<center>
![pinesMotoresPP](img/hardware/pinesMotoresPP.png)

Pines de los motores paso a paso
</center>

En el programa de control se indica la configuración de las conexiones en el **bloque inizialización**.

<center>
![confPinesMotoresPP](img/hardware/confPinesMotoresPP.png)

Configuración de las conexiones de los motores paso a paso
</center>