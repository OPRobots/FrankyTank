# BedgeTank & FrankyTank
![FrankyTank2 - Arriba](/images/Bedge-FrankyTank.jpg)

# BedgeTank (2023)
Iteración de FrankyTank, siguiendo la misma filosofía y estructura, pero con un diseño mucho más ecológico y sostenible. En lugar de bridas y varillas de fibra de carbono se usa cuerda y madera de balsa. Además, todas las piezas de PLA están impresas con filamento reciclado y se han optimizado para usar menos pegamento epoxi, manteniendo la misma rigidez y resistencia.

![BedgeTank - Abajo](/images/BedgeTank_01.jpeg)

Al igual que en la primera iteración, hemos recortado el panel solar aun más para reducir aun más el peso. También hemos optimizado el diseño de la reductora para que sea más ligera y resistente.

![BedgeTank - Reductora y Placa](/images/BedgeTank_02.jpeg)


# FrankyTank (2022)
Segundo coche solar creado por el equipo OPRobots.
El coche de este año es en esencia el mismo diseño de la ultima competición pero fabricado de 0 nuevamente. Y con algunos ajustes técnicos.

![FrankyTank2 - Arriba](/images/FrankyTank2_01.jpeg)


La premisa de este coche es la optimización de peso. Por ello el chasis del coche consiste en cuatro tubos de fibra de carbono que dan rigidez al chasis y tan solo tres ruedas: dos ruedas traseras sin transmisión y una delantera inclinada 15º que otorga la tracción y el giro.

Las ruedas traseras fueron impresas en 3D y después, con ayuda de un contramolde, se fraguó un neumatico de silicona para un agarre excepcional. La rueda delantera esta impresa en 3D, y el neumatico esta impreso con filamento extra flexible.
![FrankyTank2 - Abajo](/images/FrankyTank2_02.jpeg)

La reductora esta impresa en 3D. Tiene 2 etapas de 3:1 modificables en funcion de la radiación solar el dia de la competicion intercambiando el piñon del motor.
![FrankyTank2 - Reductora](/images/FrankyTank2_reductora.jpeg)

El coche pesa al rededor de 1100grms; para optimizar peso tambien recortamos los bordes innecesarios del panel.

Dispone de una electronica a medida ([PCB_RControl](https://github.com/OPRobots/PCB_RControl)) con PCB diseñada en KICAD mandada a fabricar a china que tambien usamos en el barco solar. Esta PCB contiene un arduino, un step, un voltimetro y amperimetro. Donde a mayores se conecta el ESC, el servo, el panel y el receptor del mando.

![FrankyTank2 - PCB Custom](/images/PCB_RContro_imagen.png)

El mando es un FlySky con un receptor que transmite por iBus recibiendo en el arduino hasta 6 canales con un solo hilo.
Con esta electronica programamos el habitual algoritmo MPPT, algunos filtros para los sensores, aceleraciones, la inicialización del Brushless, y el tratamiento de las señales del mando con nuestro software [SolarController](https://github.com/OPRobots/SolarController).
