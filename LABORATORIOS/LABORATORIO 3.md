# Laboratorio 3
---

*Tematica del laboratorio: GUÍA N° 3 – Uso de BiTalino para EMG y ECG*

## Tabla de contenidos:
---

- [Participantes](#Participantes)
- [Docentes del curso](#Docentes-del-curso)
- [Introduccion al laboratorio](#Introduccion-al-laboratorio)
- [Materiales](#Materiales)
- [Metodología](#Metodología)
- [Resultados y discusion](#Resultados-y-discusion)
- [Bibliografia](#Bibliografia)

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

## Introduccion al laboratorio (Josue)
---
<p align="justify">
  Para utilizar efectivamente intrumentación biomédica relacionada a la fisiología y la biomecánica humana, es fundamental comprender el funcionamiento de las señales biológicas y su relación con el movimiento del cuerpo. Una de las señales biológicas más importantes es el potencial de acción, que es una señal eléctrica generada por las células nerviosas y musculares al momento de generarse diversos fenomenos quimicos que afectan la permeabilidad de la membrana al sodio y al potasio. En este sentido, el Electromiograma (EMG) se ha convertido en una herramienta valiosa para la medición de la actividad eléctrica muscular, en otras palabras, es una herramienta capaz de registrar los diversos cambios de potencial y evaluar la función neuromuscular de diversas unidades motoras. Este conocimiento puede ser empleado en diversas disciplinas, como la fisioterapia, la medicina deportiva y la rehabilitación. 
  
  Dicho esto, en esta práctica de laboratorio, se tiene como objetivo explorar la generación de señales biomédicas mediante la utilización del módulo BiTalino y el software OpenSignals ,así también se espera su respectiva configuración y finalmente una correcta interpretación y utilización del módulo BiTalino como EMG para medir la actividad muscular durante la contracción voluntaria y la realización de diferentes movimientos.
  

## Materiales 
---

|  **Material**  | **Imagen referencial** |
| --- | --- |
| <p align="justify">**BITalino (r)evolution Board:** Es una placa descrita como un todo en uno para la adquisicion de bioseñales, tales como: EMG, ECG y EEG. Incluye un software OPENSOURCE para la visualizacion de las señales adquiridas </p> |<div align="center"> <img src="https://cdn.shopify.com/s/files/1/0595/1068/5887/products/BITalino-Board.1_720x.jpg?v=1646224819" width="50%" height="50%"> |
| <p align="justify">**OpenSignals Software:** Es un software Open Source que trabaja con la placa BITalino para la adquision de bioseñales.</p> |<div align="center"> <img src="https://support.pluxbiosignals.com/wp-content/uploads/2021/12/os_screens_1.jpg" width="50%" height="50%"> |
| <p align="justify">**PC y participante** Se requiere de una PC con el software descargado y un participante que actue como el paciente o sujeto de prueba.</p> |<div align="center"> <img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.coolbox.pe%2Flaptop-asus-vivobook-14--core-i5-1135g7-512gb-ssd-8gb-ram-win10-teclado-ingles-gris-11136%2Fp&psig=AOvVaw2Dj2tQJYRQjv87Er7ZOLz6&ust=1680802594948000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCMDdkt-jk_4CFQAAAAAdAAAAABAE" width="50%" height="50%"> |


##  Metodología (David y Jhoysimar)
---
<p align="justify">A continuacion, se procede a describir los pasos seguidos para el desarrollo del presente laboratorio: 
  
1. Se conecta el cable ramal de tres electrodos de medicion (Positivo, negativo y tierra) junto a sus chupones descartable a la placa BITalino para el registro de las señales EMG. El puerto de conexion se reviso en el DATASHEET del BITalino usado (PUERTO EMG).

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Materiales.jpeg" width="25%" height="25%">
</p>

2. Se coloca los electrodos en el paciente segun la siguiente imagen referencial, para la medicion del nervio mediano de la mano. 
  
<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/NERVIO_MEDIANO.png" width="50%" height="50%">
</p>

3. Se inicializa la medicion de las señales EMG del nervio mediano en el SW OpenSignals. Se configura la frecuencia de 100 Hz, ya que se encuentra dentro del rango de 2-500 Hz, el cual es el usado para la adquicion de bioseñales de tipo EMG. 

4. Se procedera a realizar 4 tipos diferentes de actividades musculares. 

<p align="center">
A. Reposo
</p>
<p align="center">
<img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/Materiales.jpeg"  width="25%" height="25%">
</p>

<p align="center">
B. Movimiento leve del dedo 
</p>

<p align="center">
C. Movimiento fuerte del dedo
</p>

<p align="center"> 
D. Contratension en el dedo 
</p>

5. Se repite el proceso para la medicion de señales EMG en el nervio tibial posterior del Soleo, tal y como se observa en la siguiente imagen referencial. 

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Imagenes/REFLEJO_H_TIBIAL_POSTERIOR.png" width="50%" height="50%">
</p>
  
Para esta medicion, 


3. Se inicializa la medicion de las señales EMG del nervio mediano en el SW OpenSignals. De este modo, obtenemos tres 
  
## Resultados y discusion (Rodolfo, Adrian)
---
<p align="justify">Ploteos finales obtenidos en Python y comparacion de los datos.</p>


<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/d3a546e23cd328f53a5a5ad6d0fe076f41d6532f/VIDEO.gif"/>
</p>
 

## Conclusiones (Mariana) 
  
Como las señales se han diferenciado. Bibliografia de por que son diferentes las señales y conclusion de las EMG. 
  
 ## Bibliografia 
