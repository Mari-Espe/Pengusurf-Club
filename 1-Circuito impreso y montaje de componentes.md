Los componentes mínimos para fabricar un robot autobalancín son: microcontrolador, motores, driver de control de los motores, un sensor que permita calcular la posición y una fuente de alimentación. Adicionalmente se pueden agregar componentes con fines estéticos y/o de filtro del voltaje para obtener señales más claras y evitar dañar el circuito.

Componentes básicos utilizados

- 1x Microcontrolador Arduino Nano
- 2x Motores paso a paso Nema 17
- 2x DRV8825
- 1x GY-521 / MPU6050
- 3x Baterías li-ion 3.7 V 4800 mAh

Componentes adicionales utilizados

- 1x Zumbador (buzzer)
- 1x resistencia 50 ohm
- 2x Condensador 100uF, 50 V
- 1x Interruptor de palanca ON/OF

El zumbador se agregó para que el robot emita un sonido al encenderse y la resistencia para regular el voltaje recibido por este. El interruptor se utilizó para poder desconectar rápidamente la alimentación del circuito y los condensadores se colocaron cercano a los drivers como parte de las recomendaciones técnicas de instalación de los mismos para evitar picos de voltaje. A continuación se muestran las conexiones del circuito:
<br>
Se cometió un error en las conexiones de SDA y SCL del driver, pues se conectaron en A6 y A7 respectivamente, cuando deberían haberse conectado a A4 y A5 por ser los pines con I2C incluido por defecto en arduino Nano. Este error se solucionó con conexiones por cable sobre la placa. 
<br>
El KiCad del proyecto se adjunta en el zip Proyecto_Pingusurf.


<img width="1696" height="789" alt="Captura de pantalla 2025-07-02 201018" src="https://github.com/user-attachments/assets/e423f82b-7fdb-4ec5-b9c1-878b3127dd1b" />


<br>
Todos los componentes se acomodaron sobre una placa de cobre y todas las conexiones antraron en una cara de la misma. Sin embargo, la placa utilizada tenía doble cara de cobre lo que supuso tiempo extra al cortar el circuito pues debió aislarse por abajo también. Para hacer los cortes por el otro lado de la cara es necesario hacer perforaciones de posición en la placa y base de corte para calzar la posición al dar vuelta la placa. <br>
<br>


<img width="843" height="841" alt="Captura de pantalla 2025-07-16 233659" src="https://github.com/user-attachments/assets/e60535db-8083-4d79-8480-e06f0aa4fe2c" />

