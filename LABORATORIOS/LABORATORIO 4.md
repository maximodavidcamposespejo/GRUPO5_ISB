# Laboratorio 4
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

## Introducción al laboratorio @Josue
---
<p align="justify">
  Para comprender la relación existente entre el comportamiento fisiológico del corazón y la lectura de señales biomédicas se hace uso de un instrumento biomédico conocido como  Electrocardiograma (ECG). El fundamento de utilización de este instrumento se basa primordialmente en conocer la anatomía y el mapeo de excitación o conducción eléctrica a lo largo de los diversos tejidos del corazón.
  
<p align="justify">
  Recordemos brevemente que la actividad eléctrica del corazón es lo que produce en sí el ECG. El sistema de conducción eléctrica del corazón está formado por varias estructuras, como el nodo sinoauricular (SA), el nodo auriculoventricular (AV), el haz de His y las fibras de Purkinje. El nodo SA es el marcapasos natural del corazón y se encarga de iniciar el latido cardíaco. A medida que la actividad eléctrica se propaga por el corazón, se produce una serie de ondas que se pueden medir a través del ECG.

<p align="justify"> 
  Por esto, se puede entender que el ECG es una herramienta útil para evaluar la salud del corazón y detectar posibles problemas cardíacos. Durante la medición del ECG, se colocan electrodos en el pecho y en las extremidades del paciente. Estos electrodos detectan la actividad eléctrica del corazón y la registran en un gráfico que muestra las diferentes ondas del ECG. Asi mismo, dicha posición de los electrodos no es arbitraria, existe una técnica de medición estándar del ECG, el cual se basa en la aplicación de 12 derivaciones para cubrir toda la información del corazón en tres direcciones. Las tres primeras derivaciones son las derivaciones bipolares, que representan el plano frontal con ambos brazos (brazo derecho = RA, brazo izquierdo = LA) y pierna izquierda (LL). Las derivaciones unipolares aumentadas de las extremidades (aVR, aVL y aVF) también representan el plano frontal y las derivaciones torácicas unipolares (V1-V6) representan el plano horizontal con electrodos colocados en seis ubicaciones en el pecho. Ver imagen como referencia.
  
<p align="center"> 
 ![image](https://user-images.githubusercontent.com/128626925/231576157-b65f1099-55a0-4f34-a45e-e45e8764d17e.png)
  <p>
  
<p align="justify">
  Dicho esto, en esta práctica de laboratorio, se tiene como objetivo explorar la generación de señales biomédicas mediante la utilización del módulo BiTalino y el software OpenSignals ,así también se espera su respectiva configuración y finalmente una correcta interpretación y utilización del módulo BiTalino como ECG para así obtener información valiosa sobre la salud cardíaca de un invididuo.
  

## Materiales 
---

|  **Material**  | **Imagen referencial** |
| --- | --- |
| <p align="justify">**BITalino (r)evolution Board:** Es una placa descrita como un todo en uno para la adquisicion de bioseñales, tales como: EMG, ECG y EEG. Incluye un software *Ipen Source* para la visualización de las señales adquiridas </p> |<div align="center"> <img src="https://cdn.shopify.com/s/files/1/0595/1068/5887/products/BITalino-Board.1_720x.jpg?v=1646224819" width="50%" height="50%"> |
| <p align="justify">**OpenSignals Software:** Es un software *Open Source* que trabaja con la placa BITalino para la adquisición de bioseñales.</p> |<div align="center"> <img src="https://support.pluxbiosignals.com/wp-content/uploads/2021/12/os_screens_1.jpg" width="50%" height="50%"> |
| <p align="justify">**PC y participante** Se requiere de una PC con el software descargado y un participante que actue como el paciente o sujeto de prueba.</p> |<div align="center"> <img src="https://coolboxpe.vtexassets.com/arquivos/ids/226222-1200-auto" width="50%" height="50%"> |


##  Metodología @David y @Jhoisymar
---
<p align="justify">A continuación, se procede a describir los pasos seguidos para el desarrollo del presente laboratorio: 
  
1. Se conecta el cable ramal de tres electrodos de medición (Positivo, negativo y tierra) junto a sus chupones descartables a la placa BITalino para el registro de las señales ECG. El puerto de conexión se reviso en la hoja de datos del BITalino usado (PUERTO ECG).

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/Materiales.jpeg" width="25%" height="25%">
</p>

2. Se colocan los electrodos en el paciente en base al manual de medicion de BITalino, para el registro de ECG. 
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/NERVIO_MEDIANO.png" width="50%" height="50%">
</p>

3. Se inicializa la medición de las señales ECG en el SW OpenSignals. Se configura la frecuencia de 100 Hz, ya que esta se encuentra dentro del rango de 1-100 Hz para electrodos superficiales.
  
4. Se procederá a realizar los siguientes pasos para el registro del ECG. 

<p align="center">
A. Reposo basal por 30 segundos.
</p>
<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/REPOSO%20NERVIO%20MEDIANO%20%E2%80%90%20Hecho%20con%20Clipchamp.gif" width="25%" height="25%">
</p>

<p align="center">
B. Ciclo de 3 repeticiones de inhalacion y exhalacion, con un aguante de 5 segundos por proceso. 
</p>
  
<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/LEVE%20NERVIO%20MEDIANO%20%E2%80%90%20Hecho%20con%20Clipchamp.gif" width="25%" height="25%">
</p>

<p align="center">
C. Reposo basal por 30 segundos.
</p>

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/FUERTE%20NERVIO%20MEDIANO%20%E2%80%90%20Hecho%20con%20Clipchamp.gif" width="25%" height="25%">
</p>

<p align="center"> 
D. Se retira los electrodos superficiales. Se procede a realizar 20 repeticiones de burpees.
</p>

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/TENSION%20NERVIO%20MEDIANO%20%E2%80%90%20Hecho%20con%20Clipchamp.gif" width="25%" height="25%">
</p>

<p align="center"> 
E. Posteriormente, se procede a grabar la señal ECG despues del ejercicio de alta exigencia.
</p>

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/TENSION%20NERVIO%20MEDIANO%20%E2%80%90%20Hecho%20con%20Clipchamp.gif" width="25%" height="25%">
</p>
  
<p align="center"> 
F. Luego de 3 minutos de reposo, procedemos a registrar otros 30 segundos de reposo
</p>

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/TENSION%20NERVIO%20MEDIANO%20%E2%80%90%20Hecho%20con%20Clipchamp.gif" width="25%" height="25%">
</p>

<p align="center"> 
G. Finalmente se procede a realizar 2 repeticiones de inhalacion y exhalacion con un aguante de 10 segundos.
</p>

<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/TENSION%20NERVIO%20MEDIANO%20%E2%80%90%20Hecho%20con%20Clipchamp.gif" width="25%" height="25%">
</p>

6. Finalmente, se exportan los canales de medición de electrodo del software OpenSignal para plotear y comparar las graficas en Python 

## Resultados y discusión @Rodolfo y @Adrian
---
<p align="justify">
Se obtuvieron los siguientes resultados:
</p>

### Ploteo de la señal obtenida en la mano

| | | |
| :---: | :---: | :---: |
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/s_mano_01.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/s_mano_02.png">|
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/s_mano_03.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/s_mano_04.png">|
</p>

### Ploteo de la señal obtenida en la pantorrilla
| | |
| :---: | :---: |
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/s_tobillo_1.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/s_tobillo_2.png">|
  
### Frecuencias de las señales obtenidas
| | |
| :---: | :---: |
|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/FFT_mano.png">|<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Lab3/FFT_tobillo.png">| 
  
El código y datos utilizados para realizar el ploteo pueden ser consultados [aquí](https://github.com/maximodavidcamposespejo/GRUPO5_ISB/tree/main/Software/Lab3). Asimismo, para el último par de imágenes, la correspondiente a la mano es la gráfica de la izquierda y la correspondiente al tobillo es la de la dererecha.

<p align="justify">
Se observan diferencias significativas en las gráficas. Respecto a las mediciones tomadas al nervio mediano en la mano, se ve que los voltajes adquiridos se incrementan con la cantidad de movimiento realizada. Caso notable es en la flexión brusca, donde se llegan a picos de 200 mV. También se puede ver un icremento de frecuencias en los periodos con mayor actividad muscular. En la primera zona de movimiento se llega a un pico de 20 Hz. En la más alta, se alcanzan 40 Hz. Sin embargo, estas se encuentran en constante oscilación de en todo momento.
  
<p align="justify">
Por su parte, en el tobillo la medición es diferente. Se ven picos de valores entre 50 a 100 milivoltios en una frecuencia que aparenta ser periódica. La diferencia con las gráficas anteriores radica en el tipo de movimiento realizado. Aunque en ambas se realizaron movimientos de flexión, en el primer experimento fueron con un movimiento continuo. En el actual, se llegaron a marcar pausas y el profesor asistió en el control de los movimientos, lo que ayudó a la formación de este tipo de ondas. 
  
<p align="justify">
Nótese también que en la segunda se alcanzó también el pico de 40 Hz en la gráfica de transformadas de Fourier. Esto muestra que lograron a obtenerse señales de frecuencia similar. Y, dentro del ámbito clínico, ambas medicones son relevantes. Las mediciones realizadas al nervio medio de la mano pueden asistir para la detección o evaluación de casos de Síndrome de Tunel Carpiano en una etapa temprana. Y las del músculo sóleo para mediciones de análisis de la marcha, regulando la coordinación motora de pacientes de un modo no invasivo y seguro.

## Conclusiones @Mariana
- Se evaluó mediante la electromiografía el comportamiento de dos músculos y células nerviosas en distintos movimientos. Para realizar este procedimiento empleamos el software OpenSignals, la placa BITalino y la guía de procedimiento de electromiografía y velocidad de conducción de nervios periféricos del ministerio de salud.

- Se logró identificar las diferencias entre cuatro movimientos realizados en el músculo abductor corto del pulgar y la conducción nerviosa motora del
nervio mediano. Se observó que en un movimiento leve la señal varia ligeramente generando picos continuos con poca intensidad, en cambio, en un movimiento más prolongado y fuerte, se generan picos de mayor intensidad. Para el caso de la contra tensión en el dedo generada por una fuerza externa, se observó que la señal presenta gran cantidad de picos intensos, continuos y prolongados. Finalmente, en el caso del reposo, se observó una señal muy cercana a 0 mV con pequeños picos que representan ruido. 
  
- Se logró identificar las diferencias entre dos diferentes movimientos realizados en el músculo síleo ubicado en la pantorrilla. En el caso del reposo, se observó una señal muy cercana a 0 mV con pequeños picos que representan ruido. En cambio, se observó que en un movimiento la señal varia generando picos continuos e intensos. Se observó que, en comparación con los picos generados por la señal del músculo abductor corto del pulgar, los obtenidos para la señal de la pantorrilla presentan una menor intensidad. 
  
  
 ## Bibliografía 
- D. C. Preston y B. E. Shapiro, “Electromyography and neuromuscular disorders : clinical-electrophysiologic-ultrasound correlations-4th edition”, p. 768.
- BITalino, “BITalino R-IoT Data Sheet,” 2020. Accessed: Apr. 05, 2023. [Online]. Available: https://www.bitalino.com/storage/uploads/media/datasheet-r-iot---v12.pdf
- Mayo Clinic: (2022). Síndrome de Túnel Carpiano - Diagnóstico y Tratamiento. [Online]. Disponible en: https://www.mayoclinic.org/es-es/diseases-conditions/carpal-tunnel-syndrome/diagnosis-treatment/drc-20355608
- Ministerio de Salud, “GUÍA DE PROCEDIMIENTO DE ELECTROMIOGRAFÍA Y VELOCIDAD DE CONDUCCIÓN DE NERVIOS PERIFÉRICOS,” Oct. 2020.
- Pineda E. E, Sabbahi M. A, Etnyre B. R. Using Standing Postures as a Practical Alternative to Gait Analysis for Assessing Normal Neuromotor Activity Variation of the Ankle Muscle Antagonists: A Soleus H-Reflex and EMG Activity Study. Int. J. Morphol.  [Internet]. 2010  Mar;  28(1): 7-12. Disponible en: http://www.scielo.cl/scielo.php?script=sci_arttext&pid=S0717-95022010000100001&lng=es.
