# Laboratorio 6
---

*Temática del laboratorio: GUÍA N° 6 – Creación de data tabular a partir de las señales fisiológicas previamente adquiridas*

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
  La tabulación y etiquetación de data es esencial para la correcta interpretación y análisis de señales biomédicas. En nuestro caso en particular, la tabulación de la data adquirida por un sensor Bitalino en modo ECG nos permitirá visualizar y analizar de forma más precisa y ordenada las señales eléctricas producidas por el corazón.
  
<p align="justify">
  También, se espera que al tabular y etiquetar de manera más precisa de los datos, esto facilite la aplicación de técnicas de machine learning en el futuro. Ya que esta herramienta es muy beneficiosa y efectiva para el conocimiento de patrones en el diagnostico de enfermedades cardíacas. 

<p align="justify"> 
  Por eso, en este laboratorio se tiene como objetivo aprender la importancia de la tabulación y etiquetación de data extraída de sensores biomédicos para aplicarla a la investigación. Para este caso, se utilizará un notebook de jupyter que contendrá la codificación necesaria para organizar y tabular nuestra data.
  
  
## Materiales 
---

|  **Material**  | **Imagen referencial** |
| --- | --- |
| <p align="justify">**BITalino (r)evolution Board:** Es una placa descrita como un todo en uno para la adquisición de bioseñales, tales como: EMG, ECG y EEG. Incluye un software *Open Source* para la visualización de las señales adquiridas </p> |<div align="center"> <img src="https://cdn.shopify.com/s/files/1/0595/1068/5887/products/BITalino-Board.1_720x.jpg?v=1646224819" width="50%" height="50%"> |
| <p align="justify">**Electrodos descartables:** Es un dispositivo médico en forma de parche adhesivo con filamentos metálicos que permiten la conducción de bioptenciales desde el paciente hacia otro dispotivo capaz de realizar la lectura de la señal. </p> |<div align="center"> <img src="https://www.almamedical.es/11317-large_default/3m-electrodos-con-soporte-de-espuma-y-tampon-abrasivo-red-dot-2259-caja-50-uds.jpg" width="50%" height="50%"> |
| <p align="justify">**OpenSignals Software:** Es un software *Open Source* que trabaja con la placa BITalino para la adquisición de bioseñales.</p> |<div align="center"> <img src="https://support.pluxbiosignals.com/wp-content/uploads/2021/12/os_screens_1.jpg" width="50%" height="50%"> |
| <p align="justify">**Jupyter:** Jupyter Notebook es una aplicación cliente-servidor permite crear y compartir documentos web en formato JSON que siguen un esquema versionado y una lista ordenada de celdas de entrada y de salida. Estas celdas albergan, entre otras cosas, código, texto (en formato Markdown), fórmulas matemáticas y ecuaciones, o también contenido multimedia. Los documentos creados en Jupyter pueden exportarse en formato HTML, PDF, Markdown o Python.</p> |<div align="center"> <img src="https://fiverr-res.cloudinary.com/images/t_main1,q_auto,f_auto,q_auto,f_auto/gigs/147298486/original/58bee033c5af267f220b23e337eb00a2c414da0c/create-python-jupyter-notebooks.jpg" width="50%" height="50%"> |
| <p align="justify">**PC y participante:** Se requiere de una PC con el software descargado y un participante que actue como el paciente o sujeto de prueba.</p> |<div align="center"> <img src="https://coolboxpe.vtexassets.com/arquivos/ids/226222-1200-auto" width="50%" height="50%"> |


##  Metodología 
---
    
<p align="justify">A continuación, se procede a describir los pasos seguidos para el desarrollo del presente laboratorio: 

1. En primer lugar, procedemos a realizar la importancion de la data adquirida de ECG durante el laboratorio 4.
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/LAB%206/Importacion%20de%20data%20y%20librerias.png" width="100%" height="100%">
</p>
  

2. Posteriormente, procedemos a la lectura de la data y su agrupación en un arreglo único.
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/LAB%206/Lectura%20y%20agrupacion.png" width="85%" height="85%">
</p>  

3. Observamos en la gráfica del arreglo el total de todos los datos registrados adquiridos durante el ECG.
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/LAB%206/PLOTEO%20DE%20DATOS.png" width="80%" height="80%">
</p>

4. Luego, se procede a graficar la señal en funcion del tiempo, para lo cual procedemos a trabajar con la frecuencia de muestreo del BITalino usado (100Hz).

5. Definimos una serie de etiquetas para la posterior tabulación.

6. Finalmente, procedemos a crear la data tabulada y etiquetada en estilo Sklearn.

  
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
No se pudo obtener con precisión la medición. Esto se debe a una mala colocación del casco en nuestro sujeto de pruebas. El ángulo de colocación es incorrecto. De acuerdo a la metodología utilizada, debería usarse un ángulo de 10/20 grados. En nuestro caso, el ángulo es de aproximadamente 30°. Esto implica que los electrodos se hayan posicionado incorrectamente, llevando a la mala medición mostrada. Ningún canal llega a mostrar ondas cerebrales y son netamente ruido.
  
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
Se procederán a analizar todas las gráficas presentadas. Comenzando por el estado basal, se ven ondas de muy baja frecuencia. Considerando que la persona que se le está midiendo debe estar en reposo, se sospecharía que se tratan de ondas alfa, las cuales tienen una frecuencia de 8 a 13 Hz. Sin embargo, se puede deducir que las ondas medidas no son de esta clase. Esto debido a que, según literatura, la onda alfa es más fácil de captar en la región occipital, raramente en la frontal donde se realizó la medición. Mientras que fue la onda de fue ritmo beta, común en la realización de EEG a adultos en reposo también.
</p>
 
  
<p align="justify">
En las ondas donde se vio mayor amplitud fue aquellas que pedían la realización de un estímulo físico, como es la apertura y cierre de ojos. Aquí se ve que la variación se debe a que el cerebro tiene que gastar menos energía en todo el proceso de entender y procesar toda la información que está siendo constantemente captada por el sentido de la vista. En cambio, al responder las preguntas la actividad es más irregular. No se distingue un patrón o guía de movimiento en estas. Pero lo que sí se puede ver es que hay mayores picos en las preguntas de mayor complejidad, debido a que la persona tuvo que pensarlas más antes de poder dar una respuesta. Por ende, su lóbulo frontal (región que, entre otras cosas, se dedica al razonamiento lógico - matemático) está realizando mayor actividad. Para esta actividad trabajó en conjunto con los lóbulos parietal y temporal.
  
  
<p align="justify">
El último punto de análisis fue la cantidad de luz emitida. Al momento de aplicarle luz de la linterna al paciente, su actividad cerebral varía significativamente. Se ven más picos y frecuencias rápidos, pese a que no se había cambiado la indicación brindada al sujeto de pruebas. Esto sirve para mostrar la interferencia de la luz en la adquisición de un correcto estado basal. Cabe resaltar que el sujeto comentaba no sentir cambio alguno al aplicarle luz a su rostro debido a la presencia de la venda. Esto señala que no es necesaria la exposición directa del paciente para que pueda haber un cambio.
</p>
  
  
Así como lo comentado la luz en el punto anterior, existen otros factores de riesgo, que también pueden traer ruido a la señal adquirida
-	Presencia de bulla en el entorno. Interfieren ya que el sentido del oído lo recibe y el cerebro también tiene que procesarlos. Podría solucionarse mediante tapones en los oídos o el uso de ruido blanco, de modo que pueda enfocarse netamente en la adquisición de señal.
-	Movimientos musculares (voluntarios o involuntarios). Estos por su propia naturaleza van a generar una bioseñal. Y como el electrodo no tiene modo de discriminarlas, pueden llegar a adquirirlas y enviarlas como si se trataran de más señales cerebrales. Gestos como sonreír o alzar una ceja ya afectarían en esto.
-	Hablar durante la medición, por las razones 
-	Hablar durante la medición, por las razones ya explicadas en el punto anterior.
-	Fuente de luz muy cercana al sujeto de pruebas, específicamente a sus ojos. La cantidad de luz causa actividad mental en el cerebro, influyendo así en la medición
- Tocar el Bitalino o un dispositivo electrónico, porque genera una diferencia de voltajes.
-	Tener al paciente de pie. Esto porque no estaría en un completo relajo, afectando a la medición

  
## Conclusiones 
  
- Se logró explorar la adquisición de señales EEG con el módulo BiTalino y el Ultracortex Mark IV, así como a procesar y analizar los datos obtenidos para el estudio de la actividad cerebral en diferentes condiciones experimentales mediante el uso de softwares como OpenSignals y OpenBCI. 
  
- Para el caso del módulo el Ultracortex Mark IV, únicamente se registró el estado basal del participante. No se logró una correcta adquisición de señal debido al incorrecto posicionamiento de los electrodos. La señal obtenida fue netamente ruido. 
  
- Para el caso del módulo BiTalino, se logró una correcta adquisición de señal. Se evaluó y analizó el comportamiento de las ondas cerebrales durante cuatro acciones diferentes: En reposo con una respiración normal y los ojos cerrados (señal basal), durante un ciclo de movimiento ocular (ciclo de OJOS ABIERTOS - OJOS CERRADOS cinco veces, manteniendo ambas fases durante cinco segundos), al resolver una serie de ejercicios matemáticos centrando la mirada en un punto fijo y al momento de aplicar luz de la linterna al paciente. Para realizar este procedimiento empleamos el software OpenSignals, la placa BITalino y la guía práctica “BITalino (r)evolution Lab Guide”.
  
- Se identificaron seis factores que pueden generar ruidos en la señal adquirida: Presencia de bulla en el entorno, movimientos musculares (voluntarios o involuntarios), hablar durante la medición, fuente de luz, tocar el Bitalino o un dispositivo electrónico, y finalmente, tener al paciente de pie. 

- Se logró experiencia obtener una comprensión más profunda del funcionamiento del cerebro y de cómo las señales biomédicas pueden aplicarse en la investigación y diagnóstico de trastornos neurológicos.

  
 ## Bibliografía 
[1] “BITalino (r)evolution Lab Guide”, 2020.
[2] Sazgar, Mona, and Michael G. Young. "Overview of EEG, electrode placement, and montages." Absolute Epilepsy and EEG Rotation Review. Springer, Cham, 2019. 117-125
[3] BITalino, “BITalino R-IoT Data Sheet,” 2020. Accessed: Apr. 05, 2023. [Online]. Available: https://www.bitalino.com/storage/uploads/media/datasheet-r-iot---v12.pdf
[4]“Jupyter Notebook: documentos web para análisis de datos, código en vivo y mucho más,” IONOS Digitalguide, Sep. 11, 2018. https://www.ionos.es/digitalguide/paginas-web/desarrollo-web/jupyter-notebook/
[5] Vijayan, S., Lepage, K. Q., Kopell, N. J., & Cash, S. S. (2017). Frontal beta-theta network during REM sleep. eLife, 6, e18894. https://doi.org/10.7554/eLife.18894
[6] Barry, R. J., Clarke, A. R., Johnstone, S. J., Magee, C. A., & Rushby, J. A. (2007). EEG differences between eyes-closed and eyes-open resting conditions. Clinical neurophysiology : official journal of the International Federation of Clinical Neurophysiology, 118(12), 2765–2773. https://doi.org/10.1016/j.clinph.2007.07.028
