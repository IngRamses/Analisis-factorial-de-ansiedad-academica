# Análisis Factorial Exploratorio: Dimensiones de la Ansiedad Académica en Estudiantes Universitarios

Este repositorio contiene el código y la explicación de un Análisis Factorial Exploratorio (AFE) realizado sobre datos simulados para identificar las dimensiones subyacentes del constructo de ansiedad académica en estudiantes universitarios.

## Descripción del Problema

La ansiedad académica es una problemática común en la educación superior que afecta negativamente el bienestar y rendimiento estudiantil (Pekrun et al., 2002) . A menudo, se aborda con estrategias generales por no comprender a fondo su estructura interna . Este proyecto busca descomponer el constructo global de "ansiedad académica" en sus componentes fundamentales para permitir intervenciones más específicas .

## Objetivo

Identificar y describir las dimensiones latentes que subyacen al constructo de ansiedad académica mediante un AFE sobre datos simulados .

## Metodología

* **Datos:** Se simularon datos (N=400) para 15 ítems de un cuestionario de ansiedad académica en escala Likert (1-5) . La simulación se diseñó intencionalmente con una estructura de 3 factores.
* **Técnica:** Se aplicó un Análisis Factorial Exploratorio (AFE) usando Python .
* **Pasos del Análisis:**
    1.  Generación de datos simulados .
    2.  Análisis Exploratorio de Datos (EDA) y cálculo de Alfa de Cronbach .
    3.  Pruebas de adecuación: Test de Bartlett y KMO .
    4.  Determinación del número de factores: Criterio de Kaiser y Gráfico de Sedimentación (Scree Plot) .
    5.  Extracción de factores con Mínimos Residuos (MINRES) y rotación Varimax .
    6.  Interpretación de factores y análisis de comunalidades.

## Resultados Principales

* **Adecuación:** Los datos fueron adecuados para el AFE (KMO = 0.907 [notebook value]; Test de Bartlett: χ²(105) = 6977.194, p < 0.001 [notebook value]). *Nota: Los valores KMO y Chi-cuadrado del notebook difieren ligeramente de los del .docx (0.916 y 6995.7), probablemente por variaciones en la simulación o cálculo. Usamos los del notebook ejecutado.*
* **Estructura Factorial:** Se identificaron **3 factores** que explican conjuntamente el **83.61%** de la varianza total .
* **Factores Identificados:**
    1.  **Miedo al Fracaso y Evaluación Social:** Preocupación por el juicio externo y expectativas (Varianza: 28.1%) .
    2.  **Dificultades de Autorregulación y Procrastinación:** Problemas de concentración, manejo de carga y postergación (Varianza: 27.9%) . *Nota: El orden/nombre puede variar ligeramente respecto al docx según las cargas exactas del notebook.*
    3.  **Ansiedad Fisiológica ante Evaluaciones:** Respuestas somáticas y cognitivas ante exámenes/presentaciones (Varianza: 27.6%) .

## Contenido del Repositorio

* `Analisis_Factorial_Ansiedad_Academica.ipynb`: Notebook de Jupyter con todo el código Python y el análisis.
* `requirements.txt`: Lista de librerías Python necesarias.
* `LICENSE`: Licencia de uso del código (MIT).
* `README.md`: Este archivo.

## Instalación y Uso

1.  Clona este repositorio: `git clone <URL_DEL_REPOSITORIO>`
2.  Crea un entorno virtual (recomendado): `python -m venv venv` y actívalo.
3.  Instala las dependencias: `pip install -r requirements.txt`
4.  Abre el notebook `Analisis_Factorial_Ansiedad_Academica.ipynb` con Jupyter Lab o Jupyter Notebook.
5.  Ejecuta las celdas para replicar el análisis. Los datos se simulan dentro del propio notebook.

## Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## Autores 


* López Soto Ramses Omar 


## Referencias

* Fabrigar, L. R., et al. (1999). Evaluating the use of exploratory factor analysis in psychological research. *Psychological Methods, 4*(3), 272–299. 
* Pekrun, R., et al. (2002). Academic emotions in students' self-regulated learning and achievement... *Educational Psychologist, 37*(2), 91-105.
