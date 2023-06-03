# Análisis básico de la señal EEG
---

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

<p align="justify">En este laboratorio, se realizó un análisis básico de la señal EEG utilizando dos datasets previamente obtenidos. Se aplicaron filtros pasabanda para identificar los ritmos cerebrales de interés y se analizó la actividad en cada banda de frecuencia. Los resultados obtenidos demostraron la presencia de los ritmos delta, theta, alpha, beta y gamma en las señales EEG analizadas. Este tipo de análisis puede ser útil para estudios posteriores relacionados con la actividad cerebral y sus correlaciones con diferentes estados mentales o trastornos neurológicos.</p>

<p align="justify">El análisis de señales de electroencefalografía (EEG) es una técnica utilizada para estudiar la actividad eléctrica del cerebro. En este laboratorio, se trabajó con dos datasets previamente obtenidos de señales EEG. Uno de ellos fue adquirido utilizando el BITalino, mientras que el otro se obtuvo mediante el dispositivo Ultracortex Mark IV. El objetivo de esta práctica es realizar un análisis básico de estas señales para identificar los ritmos cerebrales presentes.</p>

## Materiales

- BITalino
- Ultracortex Mark IV
- Jupyter Notebook con la librería biosignalsnotebooks

## Metodología

<p align="justify">1. Importación de los datasets: Se importaron los dos datasets previamente obtenidos, uno proveniente del BITalino y otro del dispositivo Ultracortex Mark IV, utilizando la librería biosignalsnotebooks en un entorno de Jupyter Notebook.</p>

<p align="justify">2. Preprocesamiento de las señales: Se realizó un preprocesamiento básico de las señales EEG. Esto incluyó la eliminación de ruido, la corrección de artefactos y la normalización de las señales.</p>

<p align="justify">3. Aplicación de filtros pasabanda: Se utilizaron filtros pasabanda para identificar los ritmos cerebrales de interés. Se establecieron las siguientes frecuencias para cada uno de los ritmos cerebrales:</p>

<p align="justify">- Delta: 0.01 - 4 Hz</p>
<p align="justify">- Theta: 4 - 8 Hz</p>
<p align="justify">- Alpha: 8 - 13 Hz</p>
<p align="justify">- Beta: 13 - 30 Hz</p>
<p align="justify">- Gamma: 30 - 49.99 Hz</p>

<p align="justify">4. Análisis de los ritmos cerebrales: Se realizó un análisis de los ritmos cerebrales presentes en las señales EEG. Se calcularon las frecuencias dominantes en cada uno de los ritmos y se generaron gráficas para visualizar la actividad en cada banda de frecuencia.</p>

## Resultados y discusión

<p align="justify">Los resultados obtenidos mostraron la presencia de distintos ritmos cerebrales en las señales EEG analizadas. A continuación, se presentan los gráficos obtenidos:</p>

### Señales obtenidas del BITalino

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/bit1.png" alt="Ondas delta">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/bit2.png" alt="Ondas theta">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/bit3.png" alt="Ondas alpha">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/bit4.png" alt="Ondas beta">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/bit5.png" alt="Ondas gamma">
</p>

### Señales obtenidas del Ulrtacortex

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/ultra1.png" alt="Ondas delta">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/ultra2.png" alt="Ondas theta">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/ultra3.png" alt="Ondas alpha">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/ultra4.png" alt="Ondas beta">
</p>

<p align="center">
  <img src="https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2011%20-%20An%C3%A1lisis%20b%C3%A1sico%20de%20la%20se%C3%B1al%20EEG/Im%C3%A1genes/ultra5.png" alt="Ondas gamma">
</p>


## Conclusiones

<p align="justify">En este laboratorio, se realizó un análisis básico de la señal EEG utilizando dos datasets previamente obtenidos. Se aplicaron filtros pasabanda para identificar los ritmos cerebrales de interés y se analizó la actividad en cada banda de frecuencia. Los resultados obtenidos demostraron la presencia de los ritmos delta, theta, alpha, beta y gamma en las señales EEG analizadas. Este tipo de análisis puede ser útil para estudios posteriores relacionados con la actividad cerebral y sus correlaciones con diferentes estados mentales o trastornos neurológicos.</p>

## Bibliografía

- Biosignalsnotebooks, “EEG - Event Related Potentials (ERP) Detection”, http://notebooks.pluxbiosignals.com/notebooks/Categories/Detect/eeg_detect_erp_rev.html (accessed Jun. 1, 2023).

- “BITalino (r)evolution Lab Guide”, 2020.

- BITalino, “BITalino R-IoT Data Sheet,” 2020. Accessed: Apr. 05, 2023. [Online]. Available: https://www.bitalino.com/storage/uploads/media/datasheet-r-iot---v12.pdf

- “Jupyter Notebook: documentos web para análisis de datos, código en vivo y mucho más,” IONOS Digitalguide, Sep. 11, 2018. https://www.ionos.es/digitalguide/paginas-web/desarrollo-web/jupyter-notebook/