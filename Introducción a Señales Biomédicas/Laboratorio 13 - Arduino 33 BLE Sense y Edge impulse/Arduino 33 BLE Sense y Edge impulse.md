# Práctica de Laboratorio 13: Arduino 33 BLE Sense y Edge Impulse

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

En esta práctica de laboratorio, se explora la integración de Arduino 33 BLE Sense con Edge Impulse, una plataforma de desarrollo de aprendizaje automático en la nube. En esta oportunidad se optó por adquirir imágenes de monedas utilizando Teachable Machine, descargarlas y luego cargarlas en Edge Impulse para crear un modelo de aprendizaje automático que pueda reconocerlas.

## Materiales
---

Los siguientes materiales se utilizaron en esta práctica de laboratorio:

- Arduino 33 BLE Sense
- Computadora con conexión a Internet
- Cables de conexión USB
- Monedas de diferentes denominaciones (10 y 50 céntimos, y 1, 2 y 5 soles)

## Metodología

1. Adquisición de imágenes de monedas utilizando Teachable Machine.

<p align="center">
  <img src="./Im%C3%A1genes/01.png" alt="Aquisición de imágenes">
</p>

2. Carga de imágenes en Edge Impulse
<p align="center">
  <img src="./Im%C3%A1genes/02.png" alt="Carga de imágenes">
</p>

3. Creación del impulso.

<p align="center">
  <img src="./Im%C3%A1genes/03.png" alt="Creación del impulso">
</p>

<p align="center">
  <img src="./Im%C3%A1genes/04.png" alt="Creación del impulso">
</p>

4. Entrenamiento del modelo.

<p align="center">
  <img src="./Im%C3%A1genes/05.png" alt="Creación del impulso">
</p>

5. Validación del modelo

<p align="center">
  <img src="./Im%C3%A1genes/06.png" alt="Validación del modelo">
</p>

6. Exportación del modelo como librería de Arduino (puede edscargarla [aquí](ei-rhuacasi-project-1-arduino.zip)).

<p align="center">
  <img src="./Im%C3%A1genes/07.png" alt="Exportación del modelo">
</p>

7. Carga y prueba del modelo en Arduino 33 BLE Sense.

## Resultados y discusión
---

Después de completar los pasos anteriores, se logró desarrollar un modelo de aprendizaje automático en Edge Impulse capaz de reconocer diferentes tipos de monedas. La precisión y el rendimiento del modelo pueden variar según la calidad de las imágenes de las monedas y la cantidad de datos de entrenamiento utilizados. Esto se evidenció cuando se testeó el modelo con imágenes de las mismas monedas pero en diferentes contextos de iluminación y fondo:

<p align="center">
  <img src="./Im%C3%A1genes/08.png" alt="Otros resultados">
</p>

Por motivos de falta de tiempo, no se pudo realizar la implementación en el Arduino 33 BLE Sense.

## Conclusiones
---

En esta práctica de laboratorio, se pudo aprender cómo utilizar Edge Impulse para crear un modelo de aprendizaje automático capaz de reconocer diferentes tipos de monedas. La integración de estas tecnologías permite el desarrollo de aplicaciones interactivas y de detección de objetos en tiempo real.

Se observó que el éxito del modelo depende en gran medida de la calidad de las imágenes de entrenamiento y la cantidad de datos utilizados. Además, se resalta la importancia de la configuración adecuada de los parámetros del modelo y la validación del mismo para lograr resultados óptimos.

## Bibliografía

- “Teachable Machine,” Google, [https://teachablemachine.withgoogle.com/](https://teachablemachine.withgoogle.com/) (accessed Jun. 23, 2023). 

- “Edge impulse,” Edge Impulse, [https://www.edgeimpulse.com/](https://www.edgeimpulse.com/) (accessed Jun. 23, 2023).

- “Detect objects with centroids,” Edge Impulse Documentation, [https://docs.edgeimpulse.com/docs/tutorials/detect-objects-using-fomo](https://docs.edgeimpulse.com/docs/tutorials/detect-objects-using-fomo) (accessed Jun. 23, 2023). 

- “Arduino nano 33 ble sense,” Arduino Online Shop, [https://store-usa.arduino.cc/products/arduino-nano-33-ble-sense](https://store-usa.arduino.cc/products/arduino-nano-33-ble-sense) (accessed Jun. 23, 2023).