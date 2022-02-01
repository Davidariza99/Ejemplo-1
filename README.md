# Proyecto embebidos (Pet_Sitting)

## Integrantes:

- David Ariza
- Andres Unibio
- Sharem Alonso

## Descripción:
Vigilante y cuidador de mascotas en casa, permite al usuario interactuar con su mascota a la distacia.

## Justificación: 
Se ha presentado un aumento significativo de la adopción de mascotas durante la pandemia, a medida que las personas vuelven a sus oficinas, universidades y demas obligaciones fuera del hogar, las mascotas que fueron criadas con la constante compañia de sus dueños, ahora sienten su ausencia. Este proyecto busca crear un nuevo vinculo entre el dueño y la mascota mientras este no se encuentre en casa

## Requerimientos funcionales:
- Vigilar 
- Comando de voz: Llamar, consentir, felicitar y corregir
- Movilidad (en un solo nivel)

## Requerimientos no funcionales:
- Cámara
- Audios pregrabados (mp3)
- Motor y alimentación
- Módulo WiFi
- Control remoto (desde un dispositivo móvil)

## Diagrama de bloques:
### Propuesto
![Diagrama_bloques drawio](/DiagramaBloques.png)
### Final
![Diagrama_bloques drawio](/Diagrama_bloques_V2.png)

## Proceso:
Ya teniendo definida la idea del proyecto, se procede a escoger cada uno de los elementos que nos permitirán realizar las tareas requeridas. Se pensó inicialmente en usar como módulo principal el ESP32, sin embargo, teniendo en cuenta el requerimiento de la cámara y que las referencias de cámara consultadas para usar en el ESP32 como la OV7670 tienen cierta complejidad al momento de configurarla y no ofrecen la mejor calidad, se decidió buscar otro módulo que contará con mejores especificaciones y facilitará el proceso. La ESP32 CAM cuenta con una cámara OV2460, que ofrece una mejor calidad y ya viene configurada a la placa.

![ESP32_CAM](/imagenes/ESP32_CAM.png)

Teniendo claro esto, lo siguiente era el desplazamiento ¿Cómo hace que esta ESP32 CAM se desplaze por el espacio para cumplir la labor de vigilancia? Se escogió un puente H conectados a dos motores que le darán esa habilidad, además de montar la tarjeta en un servo motor para tener la capacidad también de mover la cámara. 

![Puente H](/imagenes/puenteh.png)






