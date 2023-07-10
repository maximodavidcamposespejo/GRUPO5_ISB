# Curso: Introducción a Señales Biomédicas

## Design of a Wearable Electrocardigram with a predictive algorithm based on Machine Learning for Telemonitoring Coronary Heart Diseases in Peru

## Diseño de un electrocardiógrafo wearable con un algoritmo predictivo basado en Machine Learning para el telemonitoreo de enfermedades coronarias del corazón en el Perú

## Tabla de contenidos:
---

- [Resumen](#Resumen)
- [Motivación](#Motivación)
- [Principales Hallazgos](#Principales-Hallazgos)
- [Participantes](#Participantes)
- [Referencias](#Referencias)

## Resumen 
---
<p align="justify"> 
La Isquemia Miocárdica (IM) se define como una enfemedad que reduce el flujo sanguíneo en las arterias coronarias, generando muerte celular en regiones diferentes del cerebro. Al 2021, la IM registraba 22 728 muertes en el Perú. El objetivo del presente proyecto es desarrollar un algoritmo predictivo y clasificativo basado en Machine Learning para presuntos segmentos anormales en señales de electrocardiograma, que se pueden integrar en un electrocardiógrafo portátil para el telemonitoreo de pacientes on IM. 

Para la metodología, se consideraron normativas de diseño nacionales e internacionales  se diseñó una aplicación para dispositivos móviles con la función de conectar el software y hardware y ser interfaz del usuario y personal médico. Señales sinusales y bloqueos de las ramas izquierdas y derecha fueron obtenidas de una base de datos como estados de prueba para entrenar el algoritmo de Machine Learning. 

El modelo final mostró una presición de 97.2% y una pérdida del 1.0% durante el entrnamiento. Subsecuentemente, ensayos fueron realizados para evaluar su funcionamiento con una señal de ECG obtenida de un paciente varón sano de 21 años. En esta etapa, se obtuvo una presición de 95.51%, clasificándola como un ritmo sinusal normal casi completamente, lo cual coincide con la esperado.

##  Motivación 
---
<p align="justify"> 
Una enfermedad isquémica del corazón (EIC) hace referencia al estrechamiento o bloqueo de los vasos sanguíneos debido a la acumulación de una placa grasosa que se espesa y endurece en las paredes arteriales [1]. En otras palabras, una cardiopatía isquémica se produce cuando las arterias que suministran sangre al corazón se obstruyen, de manera parcial o completa, evitando un correcto suministro de sangre a los órganos y tejidos. Si esta obstrucción se da de manera lenta se le denomina angina de pecho, en cambio, si se da de forma rápida se le denomina un infarto [2]. 

Según el Repositorio Único Nacional de Información en Salud (REUNIS) en el año 2021, las EIC son la segunda causa de mortalidad nacional con un total de 22,728 defunciones, solo por detrás de la pandemia de COVID-19 con 104,348. Respecto a años anteriores, se observa que las EIC en el 2018 se reportaron 10,011 defunciones, siendo la tercera causa de mortalidad nacional; En el 2019 fueron 11,451 los fallecidos, siendo la segunda causa de mortalidad nacional; Y en el 2020 se disparó los valores a 20,522 defunciones, siendo la segunda causa a nivel nacional [3]. 

Es así que se busca desarrollar un modo de avisarle al paciente que podría tener una cardiopatía de esta índole, con un dispositivo que le muestre recomendaciones de cuando ir al médico a chequearse basado en la señal cardiaca de este.

## Principales Hallazgos
---
<p align="justify"> 
Se logró desarrollar un algoritmo que, a partir de una señal biológica de un paciente, puede filtrarla y clasificarla. Luego de esto, se segmentó y se puede definir si coincide con un ritmo cardiaco normal o alguna arrtmia, monstrándole al paciente como una sugerencia. Para esta etapa, se casificó ritmo sinusal, bloqueo de rama izquierda y bloqueo de la rama derecha.

La etapa de Machine Learning se realizó en el software Edge Impulse, donde se entrenó el modelo con una base de datos proveniente de Physionet. Se encontró precisión del 95%, un valor significativo. Este puede llegar a implementarse en un microcontrolador para un dispositivo para el paciente, como un Arduino  o ESP32.

## Participantes
---
* **Maximo David Campos Espejo** - *Collaborator* - [maximodavidcamposespejo](https://github.com/maximodavidcamposespejo)
* **Adrián Ismael Hernández Vega** - *Collaborator* - [Adrianhernandezve](https://github.com/Adrianhernandezve)
* **Rodolfo Roger Huacasi Turpo** - *Collaborator* - [berenidur](https://github.com/berenidur)
* **Josue Daniel Lachira Arellano** - *Collaborator* - [JosueLachira](https://github.com/JosueLachira)
* **Mariana Leon Prado Martínez** - *Collaborator* - [MarianaLeonPrado](https://github.com/MarianaLeonPrado)
* **Jhoisymar Eliana Ttito Herrera** - *Collaborator* - [Jhoisymar2402](https://github.com/Jhoisymar2402)

Puede encontrar más información del grupo [aquí](https://github.com/maximodavidcamposespejo/GRUPO5_ISB/blob/main/Introducci%C3%B3n%20a%20Se%C3%B1ales%20Biom%C3%A9dicas/Laboratorio%2001%20-%20Sobre%20Nosotros/Sobre%20el%20equipo.md)

## Referencias
---
[1] “Enfermedades cardiovasculares”, Paho.org. [En línea]. Disponible en: https://www.paho.org/es/temas/enfermedades-cardiovasculares. [Consultado: 09-may-2023].
[2] “Cardiopatía Isquémica”, Clínic Barcelona. [En línea]. Disponible en: https://www.clinicbarcelona.org/asistencia/enfermedades/cardiopatia-isquemica. [Consultado: 09-may-2023].
[3] Repositorio Único Nacional de Información en Salud. "Tasas de mortalidad." https://www.minsa.gob.pe/reunis/data/tasas_mortalidad.asp (consultado en mayo de 2023)
