# Laboratorio 5
---

*Tematica del laboratorio: GUÍA N° 3 – Uso de BiTalino para ECG*

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
 El EEG se compone de diferentes bandas de frecuencia que representan la actividad eléctrica del cerebro en distintos rangos de frecuencia. Estas bandas de frecuencia se clasifican en delta (0.5-4 Hz), theta (4-8 Hz), alpha (8-13 Hz), beta (13-30 Hz) y gamma (30-100 Hz), cada una con características y funciones específicas en el cerebro. Ver Tabla referencial extraída de la Guía de Bitalino,2020.


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
| <p align="justify">**OpenSignals Software:** Es un software *Open Source* que trabaja con la placa BITalino para la adquisición de bioseñales.</p> |<div align="center"> <img src="https://support.pluxbiosignals.com/wp-content/uploads/2021/12/os_screens_1.jpg" width="50%" height="50%"> |
| <p align="justify">**Fluke Prosim 4:** Es un dispositivo que permite simular signos vitales del cuerpo humano bajo parámetros regulados por el usuario.</p> |<div align="center"> <img src="https://setgad.com/wp/wp-content/uploads/2019/04/prosim4front_0.png" width="50%" height="50%"> |
| <p align="justify">**PC y participante:** Se requiere de una PC con el software descargado y un participante que actue como el paciente o sujeto de prueba.</p> |<div align="center"> <img src="https://coolboxpe.vtexassets.com/arquivos/ids/226222-1200-auto" width="50%" height="50%"> |


##  Metodología @David y @Jhoisymar
---
<p align="justify">A continuación, se procede a describir los pasos seguidos para el desarrollo del presente laboratorio: 
  
1. Se conecta el cable ramal de tres electrodos de medición (positivo, negativo y tierra) junto a sus chupones descartables a la placa BITalino para el registro de las señales ECG. El puerto de conexión se revisó en la hoja de datos del BITalino usado (PUERTO ECG).

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/Materiales.jpeg" width="25%" height="25%">
</p>

2. Se colocan los electrodos en el paciente en base al manual de medición de BITalino, para el registro de ECG.
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ECG.jpeg">
</p>

3. Se inicializa la medición de las señales ECG en el SW OpenSignals. Se configura la frecuencia de 100 Hz, ya que esta se encuentra dentro del rango de 1-100 Hz para electrodos superficiales.
  
4. Se procederá a realizar los siguientes pasos para el registro del ECG. 

<p align="center">
A. Reposo basal por 30 segundos.
</p>
<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/reposo.gif" width="25%" height="25%">
</p>

<p align="center">
B. Ciclo de 3 repeticiones de inhalación y exhalación, con un aguante de 5 segundos por proceso. 
</p>
<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/respiracion.gif" width="25%" height="25%">
</p>
  
<p align="center">
C. Reposo basal por 30 segundos.
</p>

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/reposo.gif">
</p>

<p align="center"> 
D. Se retira los electrodos superficiales. Se procede a realizar 20 repeticiones de burpees.
</p>
<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ejercicio.gif">
</p>

<p align="center"> 
E. Posteriormente, se procede a grabar la señal ECG despues del ejercicio de alta exigencia.
</p>

  
<p align="center"> 
F. Luego de 3 minutos de reposo, procedemos a registrar otros 30 segundos de reposo.
</p>

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/reposo.gif" width="25%" height="25%">
</p>

<p align="center"> 
G. Finalmente se procede a realizar 2 repeticiones de inhalación y exhalación con un aguante de 10 segundos.
</p>

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/respiracion.gif" width="25%" height="25%">
</p>

6. Finalmente, se exportan los canales de medición de electrodo del software OpenSignal para plotear y comparar las graficas en Python.

## Resultados y discusión
---
<p align="justify">
Se obtuvieron los siguientes resultados (click sobre la imagen para verla en tamaño completo):
</p>

### Ploteo de la señal obtenida antes de la actividad física

| | |
| :---: | :---: |
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg1_1.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg1_2.png">|
|La señal inicial muestra pulsos constantes. Se puede ver que en el complejo QRS se llega a picos de 200 mV. Asimismo, las ondas P y T son fácilmente apreciables. Se ve una amplitud mayor en esta última.|Al momento de inhalar y exhalar, la frecuencia de respiración y espiración es diferente. Sin embargo también se ve que esta tiene más ruido, particularmente durante las etapas de exhalación. Asimismo, se ve que en la etapa de exhalación la amplitud es ligeramente mayor.|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg1_3.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg1_0.png">|
|En este nuevo reposo, el pulso cardiaco se ha recuperado rápidamente. Tiene apariencia más similar a la señal inicialmente medida.||

### Ploteo de la señal obtenida después de la actividad física

| | |
| :---: | :---: |
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg2_1.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg2_2.png">|
|Hay diferencias significativas. El pulso es de 124 bpm aproximadamente, tratándose de una situación de taquicardia. Las ondas son mucho más rápidas. Además, la onda T se ha hecho mayor|Habiendo pasado un tiempo de reposo, la onda es más similar a la del reposo inicial. Se puede ver que hay dos amplitudes diferentes: una en las regiones de inhalación (entre 360 y 370 segundos) y otra mayor en las de exhalación, que llega a ser el doble (en 373 segundos)|

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg2_0.png"></p>
<p align="center">Las frecuencias son más variables. Puede verse picos de 6.3 Hz. Y en frecuencias mayores los valores llegan a -25 decibelios aproximadamente.</p>

### Ploteo de la señal obtenida del ProSim 4

| | |
| :---: | :---: |
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg3_1.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg3_2.png">|
|Señal normal. Puede verse como si fuera en reposo|La frecuencia se ha incrementado ligeramente|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg3_3.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg3_4.png">|
|Frecuencia mayor, similar a una etapa de ejercicio físico|La señal se va nivelando|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg3_5.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg3_6.png">|
|Señal en recuperación|Señal de vuelta a estado normal. Tras todo este ciclo, el paicente simulado está en reposo otra vez.|

<p align="center"><img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab4/ecg3_0.png"></p>
<p align="center"></p>
  
El código y datos utilizados para realizar el ploteo pueden ser consultados [aquí](https://github.com/maximodavidcamposespejo/GRUPO5_ISB/tree/main/Software/Lab4). 

<p align="justify">
Se observan diferencias significativas en las gráficas. Puede verse el aumento de frecuencia cardiaca tras actividad física y la variación de amplitud de onda en el estado de Inhalación/Exhalación. En lo que al primer caso se refiere, esto ocurre porque el corazón bombea cantidades mayores de sangre para compensar por la demanda requerida por los músculos del cuerpo, que están más activos en esta etapa. La circulación es mayor, dando pase a una situación de taquicardia. Esto puede otmar mayor o menor tiempo, dependiendo de la frecuencia con la que la persona realiza ejercicio. En el presente caso, la persona que realizó la actividad no realiza actividad física con frecuencia. Esto derivó a que su orgnaismo entre rápidamente en este estado. Para la otra situación, la diferencia radica en el intervalo R-R entre las ondas. Durante la inspiración, este se reduce. Y durante la expiración se amplía. Eso debido a que la contracción o relajación de las paredes pulmonares influje en el flujo sanguíneo. Que a su vez influye en el bombeo cardiaco.
  
<p align="justify">
Comparado con la señal generada en el dispositivo Fluke Prosim 4, se ve que estas están limpias. Es decir, que no tienen ningún ruido. En cambio, la presencia de ruido es notable en las adquiridas con BitAlino. Fuentes de este pueden deberse al movimiento involuntario propio de la persona durante la medición o al tipo de electrodos utilizados (de superficie).
  
## Conclusiones 
  
- Se evaluó mediante el electrocardiograma el comportamiento del corazón cuando la persona se encuentra en reposo con una respiración normal (señal de referencia), cuando realiza una serie de respiraciones (tres respiraciones profundas manteniendo la respiración y el reposo por cinco segundos) y después de haber realizado actividad física (20 burpees). Para realizar este procedimiento empleamos el software OpenSignals, la placa BITalino y la guía práctica “BITalino (r)evolution Lab Guide”.
  
- Se logró explorar la generación de señales biomédicas mediante la utilización del módulo BiTalino y el software OpenSignals, así también se logró una correcta configuración e interpretación módulo como ECG para así obtener información valiosa sobre la salud cardíaca de un invididuo.
  
- Se logró identificar las diferencias entre el estado de un individuo en reposo, realizando respiraciones profundas y después de realizar actividad física.  Además, se realizó una comparación de la señal obtenida mediante el dispositivo generador de signos vitales ProSim 4 de marca fluke, donde se obtuvo la señal a diferentes frecuencias. 

  
 ## Bibliografía 
- “BITalino (r)evolution Lab Guide”, 2020.
-  Sazgar, Mona, and Michael G. Young. "Overview of EEG, electrode placement, and montages." Absolute Epilepsy and EEG Rotation Review. Springer, Cham, 2019. 117-125
- BITalino, “BITalino R-IoT Data Sheet,” 2020. Accessed: Apr. 05, 2023. [Online]. Available: https://www.bitalino.com/storage/uploads/media/datasheet-r-iot---v12.pdf
- Grunovas A, Trinkunas E, Buliuolis A, Venskaityte E, Poderys J, et al. (2016) Cardiovascular Response to Breath-Holding Explained by Changes of the Indices and their Dynamic Interactions. Biol Syst Open Access 5: 152. doi:10.4172/2329-6577.1000152
- New England Baptist Hospital, "How Does Exercise Affect Your Heart, and What are the Benefits?". Accessed: Apr, 12, 2023. [Online]. Disponible en: https://www.nebh.org/blog/how-does-exercise-affect-your-heart-and-what-are-the-benefits/
