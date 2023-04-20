# Laboratorio 5
---

*Temática del laboratorio: GUÍA N° 5 – Uso de BiTalino para EEG*

## Tabla de contenidos:
---

- [Participantes](#Participantes)
- [Docentes del curso](#Docentes-del-curso)
- [Introducción al laboratorio](#Introducción-al-laboratorio)
- [Materiales](#Materiales)
- [Metodología](#Metodología)
- [Resultados y discusión](#Resultados-y-discusión)
- [Conclusiones](#Conclusiones)
- [Bibliografía](#Bibliografía)

## Participantes
---
* **Maximo David Campos Espejo** - *Collaborator* - [maximodavidcamposespejo](https://github.com/maximodavidcamposespejo)
* **Adrián Ismael Hernández Vega** - *Collaborator* - [Adrianhernandezve](https://github.com/Adrianhernandezve)
* **Rodolfo Roger Huacasi Turpo** - *Collaborator* - [berenidur](https://github.com/berenidur)
* **Josue Daniel Lachira Arellano** - *Collaborator* - [JosueLachira](https://github.com/JosueLachira)
* **Mariana Leon Prado Martínez** - *Collaborator* - [MarianaLeonPrado](https://github.com/MarianaLeonPrado)
* **Jhoisymar Eliana Ttito Herrera** - *Collaborator* - [Jhoisymar2402](https://github.com/Jhoisymar2402)

## Docentes del curso
---
* **Lewis De La Cruz**
* **Moisés Meza**
* **José Alonso Cáceres**
* **Julissa Venancio**

## Introducción al laboratorio
---
<p align="justify">
  En este laboratorio, nos enfocaremos en el uso del electroencefalograma (EEG) utilizando el módulo BiTalino, con el objetivo de adquirir y analizar las señales eléctricas del cerebro humano. El EEG es una herramienta fundamental que nos permite estudiar la actividad cerebral y comprender su funcionamiento en diferentes estados fisiológicos y patológicos.
  
<p align="justify">
  Para entender el funcionamiento del EEG, es esencial comprender la organización del cerebro humano. Este órgano está compuesto por miles de millones de neuronas que se comunican entre sí mediante impulsos eléctricos. Estos impulsos generan actividad eléctrica que puede ser registrada en la superficie del cuero cabelludo mediante electrodos estratégicamente colocados.

<p align="justify"> 
 El EEG se compone de diferentes bandas de frecuencia que representan la actividad eléctrica del cerebro en distintos rangos de frecuencia. Estas bandas de frecuencia se clasifican en delta (0.5-4 Hz), theta (4-8 Hz), alpha (8-12 Hz), beta (12-25 Hz) y gamma (25-100 Hz), cada una con características y funciones específicas en el cerebro. Ver Tabla referencial extraída de la Guía de Bitalino,2020.


  ![Captura de pantalla 2023-04-19 013309](https://user-images.githubusercontent.com/128626925/232986721-b0601ebc-0b42-415a-9495-2c817a89d794.png)

  
<p align="justify">
  La adquisición del EEG se realiza mediante la colocación de electrodos en la superficie del cuero cabelludo, los cuales registran la actividad eléctrica del cerebro en tiempo real. La organización de los electrodos sigue la organización estandarizada del Sistema Internacional 10-20, y finalmente estos electrodos estarán conectados al módulo BiTalino, un sistema de adquisición de señales biomédicas que permite capturar, amplificar y digitalizar la señal del EEG para su posterior análisis.
  
<p align="justify"> 
  En este laboratorio, aprenderemos a utilizar el módulo BiTalino para adquirir señales EEG, así como a procesar y analizar los datos obtenidos para estudiar la actividad cerebral en diferentes condiciones experimentales mediante el uso de softwares como OpenSignals y OpenBCI. Dicho esto, se espera que a través de esta experiencia obtengamos una comprensión más profunda del funcionamiento del cerebro y de cómo las señales biomédicas pueden aplicarse en la investigación y diagnóstico de trastornos neurológicos.
  
  
## Materiales 
---

|  **Material**  | **Imagen referencial** |
| --- | --- |
| <p align="justify">**BITalino (r)evolution Board:** Es una placa descrita como un todo en uno para la adquisición de bioseñales, tales como: EMG, ECG y EEG. Incluye un software *Open Source* para la visualización de las señales adquiridas </p> |<div align="center"> <img src="https://cdn.shopify.com/s/files/1/0595/1068/5887/products/BITalino-Board.1_720x.jpg?v=1646224819" width="50%" height="50%"> |
| <p align="justify">**Ultracortex Mark IV:** Es un auricular EEG impreso en 3D de código abierto diseñado para funcionar con cualquier placa OpenBCI. Permite adquirir hasta 16 canales de datos de EEG desde 35 hasta 10-20 ubicaciones diferentes. </p> |<div align="center"> <img src="https://docs.openbci.com/assets/images/UCM4-Product-2-28967dab0bd940f3b3fe67d2c7d9fcdb.JPG" width="50%" height="50%"> |
| <p align="justify">**Electrodos descartables:** Es un dispositivo médico en forma de parche adhesivo con filamentos metálicos que permiten la conducción de bioptenciales desde el paciente hacia otro dispotivo capaz de realizar la lectura de la señal. </p> |<div align="center"> <img src="https://www.almamedical.es/11317-large_default/3m-electrodos-con-soporte-de-espuma-y-tampon-abrasivo-red-dot-2259-caja-50-uds.jpg" width="50%" height="50%"> |
| <p align="justify">**OpenSignals Software:** Es un software *Open Source* que trabaja con la placa BITalino para la adquisición de bioseñales.</p> |<div align="center"> <img src="https://support.pluxbiosignals.com/wp-content/uploads/2021/12/os_screens_1.jpg" width="50%" height="50%"> |
| <p align="justify">**OpenBCI GUI:** Es un software de OpenBCI que permite visualizar, grabar y transmitir datos desde las placas OpenBCI.</p> |<div align="center"> <img src="https://docs.openbci.com/assets/images/GUI-V4-Screenshot-6d16898fb8d30a8f48e2f748ff0c2d51.jpg" width="50%" height="50%"> |
| <p align="justify">**PC y participante:** Se requiere de una PC con el software descargado y un participante que actue como el paciente o sujeto de prueba.</p> |<div align="center"> <img src="https://coolboxpe.vtexassets.com/arquivos/ids/226222-1200-auto" width="50%" height="50%"> |


##  Metodología 
---
<p align="justify">A continuación, se procede a describir los pasos seguidos para el desarrollo del presente laboratorio: 

**Medicion empleand OpenBCI GUI:**
  
1. Para adquirir el electroencefalograma (EEG) se coloca el ultracortex Mark IV en la cabeza del participante, el ultracortex Mark IV emplea el Sistema internacional 10–20 para el posicionamiento de los electrodos.

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/Sistema%2010-20.png" width="35%" height="35%">
</p>


2.  Se procede a adquirir la señal en estado basal durante 30 segundos. Para este laboratorario en particular, debido al poco tiempo disponible con el Ultracortex y los problemas iniciales de conexion, solo se pudo registrar un tiempo corto menor a 10 segundos. En la imagen 2 se observa como queda el dispositivo de medicion EEG sobre el participante.
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/Posicion%20electrodos.jpeg" width="25%" height="25%">
</p>
  
**Medicion empleando BITalino:**
    
1. Se procede a usar, como en laboratorios anteriores, el kit BITalino con el puerto de medicion EEG. La posicion de los electrodos se basa en la siguiente imagen referencial, extraida de la guia de uso de BITalino para mediciones EEG.

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/POSICIONAMIENTO%20ELECTRODOS%20BITALINO.jpg" width="35%" height="35%">
</p>

2.  Registrar una línea base de señal con poco ruido y sin movimientos (respiración normal, sin movimientos oculares/ojos cerrados) durante 30 segundos
  
<p align="center">

https://user-images.githubusercontent.com/128626554/233225137-070fa709-75ec-4dae-ab64-bc1c70f650ae.mp4
  
</p>
  
3. Registrar un ciclo de 5 repeticiones de un ciclo de OJOS ABIERTOS y OJOS CERRADOS ,manteniendo 5 segundos por proceso. 

<p align="center">
  
https://user-images.githubusercontent.com/128626554/233225219-953b87f2-aaae-43d0-a441-a742b79bd3a7.mp4
  
</p>
  
4. Registrar nuevamente una fase de reposo basal por 30 segundos.

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/4%20basal.jpg" width="35%" height="35%">
</p>

5. Registrar , con el participante con los ojos cerrados, una serie de 5 preguntas de razonamiento matematico y observar la variacion en las ondas. Las preguntas utilizadas se detallan a continuacion.
<p align="center">

https://user-images.githubusercontent.com/128626554/233225332-006500b2-e174-4aa4-b6cb-ac6ea6498049.mp4  
  
</p>

6. Luego de guardar las mediciones realizadas, se procedera a vendar los ojos del participante y registrar el estado basal (Con el menor ruido posible) por 1 minuto aproximadamente.
<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/6%20VENDAR%20OJOS.jpg" width="35%" height="35%">
</p>

7. Posterior al minuto, se procedera a encender las luces del flash del celular y pasarlo por el rostro del participante vendado. 
<p align="center">

https://user-images.githubusercontent.com/128626554/233225375-18bc765d-6453-43f6-a708-94a316eec952.mp4
  
</p>
  
8. Finalmente, se detiene la grabación y se exportan los canales de medición de electrodo del software OpenSignal para plotear y comparar las graficas en Python.
  
## Resultados y discusión
---
<p align="justify">
Se obtuvieron los siguientes resultados (click sobre la imagen para verla en tamaño completo):
</p>
  

### Ploteo de la señal obtenida con el Ultracortex Mark IV

| | |
| :---: | :---: |
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/ultracortex0.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/ultracortex1.png">|
|Canal 0|Canal 1|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/ultracortex2.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/ultracortex3.png">|
|Canal 2|Canal 3|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/ultracortex4.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/ultracortex5.png">|
|Canal 4|Canal 6|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/ultracortex6.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/ultracortex7.png">|
|Canal 6|Canal 7|
 
<p align="justify">
No se pudo obtener con precisión la medición. Esto se debe a una mala colocación del casco en nuestro sujeto de pruebas. En la imagen puede verse que el ángulo de colocación es incorrecto. De acuerdo a la metodología utilizada, debería usarse un ángulo de 10/20 grados. En nuestro caso, el ángulo es de aproximadamente 30°. Esto implica que los electrodos se hayan posicionado incorrectamente, llevando a la mala medición mostrada. Ningún canal llega a mostrar ondas cerebrales y son netamente ruido.
  
</p>

### Ploteo de la señal obtenida con el Bitalino

| | |
| :---: | :---: |
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino00.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino01.png">|
|Primer estado basal. Duración 30 segundos|Serie de repeticiones de cerrar los ojos 5 segundos y luego abrirlos|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino02.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino03.png">|
|Segundo estado basal. duración 30 segundos|Pregunta simple 1|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino04.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino05.png">|
|Pregunta simple 2|Pregunta simple 3|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino06.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino07.png">|
|Pregunta simple 4|Pregunta compleja 1|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino08.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino09.png">|
|Pregunta compleja 2|Pregunta compleja 3|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino10.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab5/bitalino11.png">|
|Cerrar los ojos vendados|Aplicar las lujces a ojos vendados|


El código y datos utilizados para realizar el ploteo pueden ser consultados [aquí](https://github.com/maximodavidcamposespejo/GRUPO5_ISB/tree/main/Software/Lab5). 

<p align="justify">
Se procederán a analizar todas las gráficas presentadas. Comenzando por el estado basal, se ven ondas de muy baja frecuencia. Cosniderando que la persona que se le está midienod debe estar en reposo, se sospecharía que se tratan de ondas alfa, las cuales tienen una frecuencia de 8 a 13 Hz. 
</p>
 
<p align="justify">
Sin embargo, se puede decucir que las ondas medidas no son de esta clase. Esto debido a que según literatura, la onda alfa es más fácil de captar en la región occipital, raramente en la frontal donde se realizó la medición. Mientras que fue la onda de fue ritmo beta, común en adultos en reposo también.
</p>
 
<p align="justify">
En las ondas donde se vio mayor amplitud fue aquellas que pedían la realizaión de un estínulo físico, como es la apertura y cierre de ojos. En cambio, al responder las preguntas la activdad es más irregular. No se distingue un patrón o guía de movimiento. Pero lo que sí se puede ver es que hay mayor frecuencia en las preguntas de mayor dificultad, debido a que tuvo que pensarlas más antes de poder dar una respuesta.
</p>
  
<p align="justify">
El último punto de análisis fue la cantidad de luz emitida. Al momento de aplicarle luz de la linterna al paciente, su actividad cerebral varía significativaemnte. Se ven más picos y frecuencias rápidos, pese a que no se había cambiado la indicación brindada al sujeto de pruebas. Esto sirve para mostrar la interferencia de la luz en la adquisición de un correcto estado basal.
</p>
  
<p align="justify">
Así como la luz en el punto anterior, existen otros factores de riesgo, que también pueden traer ruido a la señal adquirida
  -	Presencia de bulla en el entorno. Podría solucionarse mediante tapones en los oídos o el uso     de ruido blanco
  -	Movimientos musculares (voluntarios o involuntarios)
  -	Hablar durante la medición
  -	Fuente de luz muy cercana al sujeto de pruebas, específicamente a sus ojos
  -     Tocar el Bitalino
  -	Estar de pie

</p>
  
## Conclusiones 
  
- Se logró explorar la generación de señales biomédicas mediante la utilización del módulo BiTalino y el software OpenSignals, así también, se logró una correcta configuración e interpretación del módulo como EEG. Ouede verse una circulación tranquila, pero al ser distntas generacioes, variará un poco ka adquisición
  
- Se evaluó y analizó mediante el electroencefalograma el comportamiento del cerebro durante tres acciones diferente: En reposo con una respiración normal y los ojos cerrados (señal basal), durante un ciclo de movimiento ocular ( ciclo de OJOS ABIERTOS - OJOS CERRADOS cinco veces, manteniendo ambas fases durante cinco segundos), y al resolver una serie de ejericios mátematicos centrando la mirada en un punto fijo. Para realizar este procedimiento empleamos el software OpenSignals, la placa BITalino y la guía práctica “BITalino (r)evolution Lab Guide”.
  
- Se logró identificar las diferencias entre hombre enamorado de btaman y aquel enfermo en las filipinas. Puede verse una onda amplia. Asimismo, el cambio notorio al hacerte preuntas. La variación que diga "Y fronto me veran" Y prodcedimos a tomarnos aquella foto.

  
 ## Bibliografía 
- “BITalino (r)evolution Lab Guide”, 2020.
-  Sazgar, Mona, and Michael G. Young. "Overview of EEG, electrode placement, and montages." Absolute Epilepsy and EEG Rotation Review. Springer, Cham, 2019. 117-125
- BITalino, “BITalino R-IoT Data Sheet,” 2020. Accessed: Apr. 05, 2023. [Online]. Available: https://www.bitalino.com/storage/uploads/media/datasheet-r-iot---v12.pdf
- OpenBCI, “The OpenBCI GUI | OpenBCI Documentation,” openbci.github.io, Jan. 02, 2023. https://docs.openbci.com/Software/OpenBCISoftware/GUIDocs/#:~:text=The%20OpenBCI%20GUI%20is%20OpenBCI (accessed Apr. 19, 2023).
- Grunovas A, Trinkunas E, Buliuolis A, Venskaityte E, Poderys J, et al. (2016) Cardiovascular Response to Breath-Holding Explained by Changes of the Indices and their Dynamic Interactions. Biol Syst Open Access 5: 152. doi:10.4172/2329-6577.1000152
- New England Baptist Hospital, "How Does Exercise Affect Your Heart, and What are the Benefits?". Accessed: Apr, 12, 2023. [Online]. Disponible en: https://www.nebh.org/blog/how-does-exercise-affect-your-heart-and-what-are-the-benefits/
