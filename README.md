# Sistema Difuso para la Estimación del Valor de Mercado en el Fútbol

Este repositorio contiene el desarrollo e implementación de un **Sistema de Inferencia Difuso (Fuzzy Inference System - FIS)** diseñado para estimar el valor de mercado de jugadores de fútbol profesionales. El modelo combina lógica difusa con datos reales y tangibles, alejándose de valoraciones puramente subjetivas para ofrecer un enfoque más estructurado y analítico.

## Objetivo del Proyecto

El objetivo principal es modelar de manera matemática y difusa cómo diversas métricas de rendimiento deportivo y contexto afectan el valor económico de un futbolista en el mercado actual. Se busca crear un sistema que asimile la lógica humana utilizada por analistas, ojeadores y directivos, aplicando reglas de inferencia precisas.

## Enfoque Técnico y Metodología

El proyecto utiliza un sistema de inferencia **Mamdani** implementado mediante herramientas de lógica difusa (como Matlab Fuzzy Logic Toolbox). Se definen variables lingüísticas y funciones de pertenencia (trapezoidales y triangulares) para modelar la incertidumbre del mercado.

El sistema se alimenta de tres **variables de entrada** fundamentales:
- **Edad (15 - 42 años):** Categorizada en *Talento, Joven, Prime, Veterano* y *Retirada*. Modela la curva natural de valor de un jugador a lo largo de su carrera deportiva.
- **Rendimiento (0 - 10):** Basado en las calificaciones objetivas de portales estadísticos como **WhoScored**. Sus conjuntos son *Malo, Normal, Bueno* y *Alto*.
- **Equipo (0 - 260 puntos):** Basado en el coeficiente de clubes de la **UEFA**. Evalúa el prestigio, la exposición y el nivel competitivo del club de procedencia (*Pequeño, Competitivo, Grande*).

La **variable de salida** es el:
- **Valor de Mercado (0 - 250 millones de €):** Estimación económica del jugador, clasificada en *Residual, Bajo, Medio, Alto* y *Superestrella*.

El comportamiento del sistema está regido por un conjunto de **reglas difusas** (mediante operadores lógicos, métodos de agregación y defusificación por centroide) que interrelacionan estas entradas para determinar la tasación final.

## Estructura del Repositorio

- `mercado_jugador.fis` / `MercadoFutbol.fis` / `ejemplo_FUZZY.fis`: Archivos del sistema de inferencia difuso que contienen las variables, las funciones de pertenencia y las reglas. Pueden ser importados y simulados en herramientas compatibles como Matlab (Fuzzy Logic Designer).
- `Sistema Difuso - Valor de Mercado de un jugador.pdf`: **Memoria técnica y documento principal del proyecto**. 

## Documentación Detallada

Para una comprensión en profundidad sobre las decisiones de diseño, la configuración exacta de las funciones de pertenencia, la tabla de reglas de inferencia y los casos de prueba simulados con jugadores reales, es **altamente recomendable** consultar el informe técnico completo incluido en el repositorio: 

📄 **[Sistema Difuso - Valor de Mercado de un jugador.pdf](./Sistema%20Difuso%20-%20Valor%20de%20Mercado%20de%20un%20jugador.pdf)**

## Autores

Proyecto desarrollado para la asignatura de **Representación del Conocimiento y Razonamiento Automático** por:
- David Diz Oubiña
- Mateo Freire Espasandín
- Jesús Porteiro Carro
- Sergio Rego Criado
- Jorge García Varela
