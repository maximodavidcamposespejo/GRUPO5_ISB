# Laboratorio 7
---

*Temática del laboratorio: GUÍA N° 7 – Creación de filtros digitales*

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
  En este laboratorio, nos enfocaremos en el procesamiento de señales de electrocardiograma (ECG) y cómo aplicar técnicas de filtrado para reducir el ruido presente en las señales.
  
<p align="justify">
  En el laboratorio anterior, aprendimos la importancia de la tabulación y etiquetación de los datos de ECG para su posterior análisis. Ahora, utilizaremos los datos organizados y etiquetados para aplicar técnicas de filtrado. 

<p align="justify"> 
 Es importante entender que las señales de ECG pueden contener ruido debido a diversas fuentes, como interferencias electromagnéticas, movimiento del paciente o el propio equipo de medición. Por lo tanto, es crucial aplicar técnicas de filtrado para eliminar este ruido y obtener una señal de ECG más clara y precisa.

<p align="justify"> 
 En este laboratorio, nos enfocaremos en los filtros FIR (Respuesta al Impulso Finita) y los filtros IIR (Respuesta al Impulso Infinita) para el procesamiento de señales de ECG. Los filtros FIR utilizan una respuesta al impulso finita para filtrar las señales de ECG, mientras que los filtros IIR utilizan una respuesta al impulso infinita para procesar las señales 

<p align="justify">
Es importante entender las diferencias entre estos dos tipos de filtros y cómo se pueden aplicar de manera efectiva en el procesamiento de señales de ECG.
  
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

1. En primer lugar, procedemos a realizar la creación de los distintos tipos de filtros IIR (Bessel, Butterworth y Chebyshev 1) y FIR (Hamming y Blackman) mediante el uso de pyFDA. A continuación, se observa una gráfica ejemplo usando los siguientes parámetros:

<p align="center">
  Fc = 20 hz
  ; Wp = 94 rad/s
  ; Ws = 157 rad/s
</p>
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/IIR_BESSEL_2.png" width="100%" height="100%">
</p>

Algunas consideraciones adicionales tomadas para la creación de los filtros es el uso del orden mínimo requerido para la obtención de un filtro adecuado.

2. Posteriormente, procedemos a utilizar los parámetros y coeficientes derivados de la creación del filtro anteriormente mencionado, para el diseño del filtro en python.
  
3. Luego, usando el laboratorio pasado de etiquetación y creación de segmentos de data, procedemos a filtrar la señal ECG obtenida y verificar la diferencia entre la aplicación de los diferentes filtros FIR e IIR. 

4. Finalmente, procedemos a seleccionar únicamente los 2 mejores filtros (Uno FIR y otro IIR) y procedemos a aplicarlo en las categorías de señales observadas y detalladas en la siguiente imagen (Categorías creadas la anterior sesión de laboratorio)
 
|**Descripción**|**Categoría**|
| ------------- | ------------- |
| Basal 1 | 0 |
| Inhalación y exhalación| 1 |
| Basal 2 | 2 |
| Reposo 1 | 3 |
| Reposo 2 | 4 |

- **Basal 1**: Primera medición realzada, cuando el sujeto de pruebas está en reposo.
- **Inhalación y exhalación**: Ciclo de repeticiones de inhalación y exhalación, con un aguante de 5 segundos por proceso.
- **Basal 2**: Segunda medición en reposo basal.
- **Reposo 1**: Medición del reposo inmediatamente después del ejercicio de alta exigencia.
- **Reposo 2**: Medición del reposo 3 mintos después del ejercicio de alta exigencia.
  
## Resultados y discusión
---
<p align="justify">
Se obtuvieron los siguientes resultados (click sobre la imagen para verla en tamaño completo):
</p>

### Señal filtrada

| Campo | Señal cruda | Filtro IIR (Blackman) | Filtro FIR (Butterworth) |
| :--- | :---: | :---: | :---: |
| Basal | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg00.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg01.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg02.png"> |
| Respiración | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg10.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg11.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg12.png"> |
| Post-Ejercicio | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg20.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg21.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/ecg22.png"> |

### FFT

| Campo | Señal cruda | Filtro IIR | Filtro FIR |
| :--- | :---: | :---: | :---: |
| Basal | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft00.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft01.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft02.png"> |
| Respiración | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft10.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft11.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft12.png"> |
| Post-Ejercicio | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft20.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft21.png"> | <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/Im%C3%A1genes/fft22.png"> |

El código y datos utilizados para realizar el ploteo pueden ser consultados [aquí](https://github.com/maximodavidcamposespejo/GRUPO5_ISB/tree/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%207%20-%20Filtros%20digitales/C%C3%B3digo).

<p align="justify">
Lo primero que debe comentarse es los tipos de ventanas de los filtros utilizados. Para el filtro FIR se usó la ventana Blackman y para el IIR Butterworth.
  
En el caso de Blackman esta está regida por la ecuación que se ve abajo y se la consideró para el presente proyecto porque esta puede reducir los lóbulos lateriales y permite en partes el aliasing de la señal, atenuando sus valores. Con esto se puede eliminar eficazmente las frecuencias no deseadas, razón por la cual es ampliante usado en la industria de audio.
  
</p>
  
<p align="center">
w(n) = 0.42 - 0.5cos(2*pi*n/M) + 0.08cos(4*pi*n/M)
</p>
 
<p align="justify">
En la ecuación anterior, M respresenta la cantidad de elementos de la ventana cuyos valores son definidos por el usuario, los cuales se usaban para aliasing. En la presente actividad logró darse el filtrado, como se ve líneas arriba. Las frecuencias menores lograron ser eliminadas. Para mostrar esto con mayor claridad, se usó la Transformada Rápida de Fourier (FFT). Ahora en el dominio de la frecuencia, se pudo ver que para todas las categorías la frecuencia de corte está alrededor de los 20Hz. Efectivamente, el filtro pasabajas funciona.
  
Pasando al filtro de Butterworth, su respuesta en magnitud es ligeramente diferente.También descensos menos proununciados. Analizando las imágenes hay un detalle: y es que en la región de aproximadamente 15Hz, hay un pequeño pronunciamiento en la gráfica. Pasando por el dominio de la freucencia, se peude ver que ambos filtros son prácticamente iguales, pero puede notarse que al final de la región de corte (aprox 20 Hz), mientras se estabiliza y desciende aparece un rizado ligeramente pronunciado. Esto depende de las características de los diveros dispositivos disponibles que el filtrado de señales digitales.
</p>

## Conclusiones 
  
- Se logró la visualización, clasificación y análisis de un ECG empleando la tabulación y etiquetación de datos a través del notebook jupyter. 
  
- Se identificó y comprendió el proceso tabulación y etiquetación de datos como parte del proceso de tratamiento de señales biomédicas.
  
- Se logró obtener resultados correctamente clasificados en los diferentes tipos de señal adquiridas (basal, post-ejercicio, basal2, reposo 1 y resposo2) lo que facilita la implementación de técnicas de machine learning en el futuro. 

  
 ## Bibliografía 
- “BITalino (r)evolution Lab Guide”, 2020.

- BITalino, “BITalino R-IoT Data Sheet,” 2020. Accessed: Apr. 05, 2023. [Online]. Available: https://www.bitalino.com/storage/uploads/media/datasheet-r-iot---v12.pdf

- DSPrelated, "Use of a Blackman Window," [Online]. Available: https://www.dsprelated.com/freebooks/mdft/Use_Blackman_Window.html
  
- “Jupyter Notebook: documentos web para análisis de datos, código en vivo y mucho más,” IONOS Digitalguide, Sep. 11, 2018. https://www.ionos.es/digitalguide/paginas-web/desarrollo-web/jupyter-notebook/
 
- Mathworks, "butter" 
 
- Python, "scipy.signal.windows.blackman" [Online]. Available: https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.windows.blackman.html
