# Análisis básico de la señal EMG
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

<p align="justify">En este laboratorio, se llevó a cabo un análisis básico de la señal electromiográfica (EMG, por sus siglas en inglés) utilizando dos datasets previamente obtenidos. Estos datasets consistían en señales EMG de la mano y el tobillo respectivamente. El objetivo principal de esta práctica fue analizar los períodos de activación en las señales EMG y determinar su inicio y fin.</p>

## Materiales
---

<p align="justify">- Datasets de señales EMG de mano y tobillo.</p>
<p align="justify">- Computadora con Python y Jupyter Notebook instalados.</p>
<p align="justify">- Biblioteca de procesamiento de señales biosignalsnotebooks.</p>

## Metodología
---

<p align="justify">1. Carga de los datasets: Se importaron los datasets de señales EMG de mano y tobillo previamente obtenidos en formato adecuado para su procesamiento.</p>

<p align="justify">2. Preprocesamiento de la señal: Se realizó un preprocesamiento de la señal utilizando la librería biosignalsnotebooks. Esta incluye una guía para el procesamiento de señales EMG y proporciona funciones para aplicar un filtro pasabanda, así como el operador TKEO (Teager-Kaiser Energy Operator) y una fase de suavizado. Esta función fue modificada para utilizar un filtro pasaaltas con una frecuencia de corte de 10Hz, debido a que la frecuencia de sampleo del dataset fue de 100Hz.</p>

<p align="justify">3. Detección de períodos de activación: Se definió un límite de detección (del 10%, relativo al valor medio de la señal suavizada) para identificar los períodos de activación en la señal EMG. Utilizando las funciones proporcionadas por la librería, se detectaron los períodos de activación y se determinó su inicio y fin.</p>

<p align="justify">4. Análisis de resultados: Se analizaron los resultados obtenidos, observando los períodos de activación identificados en la señal EMG de mano y tobillo. Se compararon los patrones de activación y se realizaron inferencias sobre la actividad muscular correspondiente.</p>

## Resultados y discusión
---

<p align="justify">Los resultados obtenidos mostraron claramente los períodos de activación en las señales EMG de mano y tobillo. A través del análisis de los patrones de activación, se pudo inferir la actividad muscular correspondiente en cada caso.</p>

<p align="justify">En la señal EMG obtenida de la mano, se observaron períodos de activación consistentes con la contracción y relajación de los músculos, lo que indica la realización de movimientos. De igual manera con la señal EMG obtenida del tobillo.</p>

<p align="justify">La detección precisa de los períodos de activación en las señales EMG es fundamental para comprender la actividad muscular y su relación con los movimientos realizados. Este análisis básico proporciona una visión general de la señal EMG y sienta las bases para análisis más avanzados y específicos en el campo de la biomecánica y la fisiología muscular.</p>

## Conclusiones
---

<p align="justify">En esta práctica de laboratorio, se realizó un análisis básico de la señal EMG utilizando dos datasets de señales EMG de mano y tobillo. Mediante el procesamiento de la señal y la detección de períodos de activación, se logró identificar y analizar los momentos de actividad muscular en cada caso.</p>

<p align="justify">El análisis de la señal EMG es de gran relevancia en el campo de la biomecánica y la fisiología muscular, ya que proporciona información valiosa sobre la actividad muscular y su relación con los movimientos del cuerpo. Este análisis básico sienta las bases para investigaciones más avanzadas y específicas en estas áreas.</p>

## Bibliografía
---

- Biosignalsnotebooks, “Event Detection - Muscular Activations (EMG),” detect_bursts, http://notebooks.pluxbiosignals.com/notebooks/Categories/Detect/detect_bursts_rev.html (accessed Jun. 2, 2023).

- “BITalino (r)evolution Lab Guide”, 2020.

- BITalino, “BITalino R-IoT Data Sheet,” 2020. Accessed: Apr. 05, 2023. [Online]. Available: https://www.bitalino.com/storage/uploads/media/datasheet-r-iot---v12.pdf

- “Jupyter Notebook: documentos web para análisis de datos, código en vivo y mucho más,” IONOS Digitalguide, Sep. 11, 2018. https://www.ionos.es/digitalguide/paginas-web/desarrollo-web/jupyter-notebook/
