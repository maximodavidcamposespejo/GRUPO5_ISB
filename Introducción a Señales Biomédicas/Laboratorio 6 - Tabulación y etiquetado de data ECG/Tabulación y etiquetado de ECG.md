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
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/Importando%20data%20y%20librerias.png" width="100%" height="100%">
</p>
  

2. Posteriormente, procedemos a la lectura de la data y su agrupación en un arreglo único. Ademas, segmentamos la data en grupos dependiendo de la categoria a la que pertenezca
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/Lectura%20y%20agrupacion%20de%20datos.png" width="85%" height="85%">
</p>  

3. Observamos en la gráfica del arreglo el total de todos los datos registrados adquiridos durante el ECG. Se observa un ejemplo correspondiente al estado basal inicial durante los ejercicios realizados en el laboratorio 4
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/Primer%20plot.png" width="80%" height="80%">
</p>

4. Luego, se procede a obtener la señal en funcion del tiempo, para lo cual procedemos a trabajar con la frecuencia de muestreo del BITalino usado (100Hz).

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/Frecuencia%20tiempo.png" width="80%" height="80%">
</p>

5. Definimos una serie de etiquetas para la posterior tabulación.

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/etiquetas.png" width="80%" height="80%">
</p>

6. Finalmente, procedemos a crear la data tabulada y etiquetada en estilo Sklearn.

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/concatenando.png" width="80%" height="80%">
</p>
  
## Resultados y discusión
---
<p align="justify">
Se obtuvieron los siguientes resultados (click sobre la imagen para verla en tamaño completo):
</p>

### Ploteo de todos los registros obtenidos con el ECG

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/Plots.png" width="80%" height="80%">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/plots2.png" width="80%" height="80%">
</p>

### Tabla construida con los datos clasificados

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Im%C3%A1genes/Resultado%20final.png" width="80%" height="80%">
</p>

<p align="justify">
Para realizar esta clasificación se guió de la siguiente tabla, definida por el grupo a partir de los cinco tipos de señales adquiridas. Estos tipos y lo que representan se explican a continuación:

|**Descripción**|**Categoría**|
| ------------- | ------------- |
| Basal 1 | 0 |
| Post-ejercicio| 1 |
| Basal 2 | 2 |
| Reposo 1 | 3 |
| Reposo 2 | 4 |

 
<p align="justify">
- **Basal 1**: Primera medición realzada, cuando el sujeto de pruebas está en reposo.
- **Post-ejercicio**: Ciclo de repeticiones de inhalación y exhalación, con un aguante de 5 segundos por proceso.
- **Basal 2**: Segunda medición en reposo basal.
- **Reposo 1**: Medición del reposo inmediatamente después del ejercicio de alta exigencia.
- **Reposo 2**: Medición del reposo 3 mintos después del ejercicio de alta exigencia.

<p align="justify">
Se puede ver que toda la data ha sido clasificada con éxito. Nótese que los grupos 3 y 4 tienen mayor cantidad de elementos que los otros. esto se debe a que estos dos fueron tomadas en una etapa en la que el corazón se estaba recuperando del ejercicio, razón por la que había una frecuencia cardiaca notablemente mayor.</p>
 

El [código](https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/C%C3%B3digo/Pasando%20a%20data%20tabular.ipynb) y [datos utilizados para realizar el ploteo](https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%206%20-%20Tabulaci%C3%B3n%20y%20etiquetado%20de%20data%20ECG/Data) pueden ser revisados aquí.

  
## Conclusiones 
  
- Se logró la visualización, clasificación y análisis de un ECG empleando la tabulación y etiquetación de datos a través del notebook jupyter. 
  
- Se identificó y comprendió el proceso tabulación y etiquetación de datos como parte del proceso de tratamiento de señales biomédicas.
  
- Se logró obtener resultados correctamente clasificados en los diferentes tipos de señal adquiridas (basal, post-ejercicio, basal2, reposo 1 y resposo2) lo que facilita la implementación de técnicas de machine learning en el futuro. 

  
 ## Bibliografía 
- “BITalino (r)evolution Lab Guide”, 2020.

- BITalino, “BITalino R-IoT Data Sheet,” 2020. Accessed: Apr. 05, 2023. [Online]. Available: https://www.bitalino.com/storage/uploads/media/datasheet-r-iot---v12.pdf

- “Jupyter Notebook: documentos web para análisis de datos, código en vivo y mucho más,” IONOS Digitalguide, Sep. 11, 2018. https://www.ionos.es/digitalguide/paginas-web/desarrollo-web/jupyter-notebook/
