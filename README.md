
# AnaliticaPredictiva TrabajoFinal
Se desarrolló un modelo de aprendizaje automático de tipo clasificación para predecir el resultado de aprobación de estudiantes en el primer ciclo universitario.

El estudio se basó en un conjunto de datos generales, encuestas de hábitos de estudio y resultados de análisis psicopedagógicos de los estudiantes del primer ciclo de carreras de ingeniería en una universidad de El Salvador.

Se confirmaron hipótesis respecto a las relaciones entre las variables involucradas, y a la vez se encontraron correspondencias no previstas entre las variables de estudio.

El estudio se basó en un conjunto de datos generales, encuestas de hábitos de estudio y resultados de análisis psicopedagógicos de los estudiantes del primer ciclo de carreras de ingeniería en una universidad de El Salvador.

## Integrantes
*  Marvin López Osorio
*  Eduardo Rivera

## Objetivo
Predecir si un estudiante reprobará el primer ciclo universitario mediante un modelo de clasificación basado en variables psicopedagógicas, conductuales (malos hábitos) y generales.

## El dataset original continene las siguientes variables:

Ingreso,
Estado,
Sexo,
Municipio,
Edad,
Paes,
Carrera,
Facultad,
Segunda carrera,
CUM,
Porcentaje de avance,
Estado actual,
Razonamiento Verbal (DAT- VR),
Relaciones Espaciales (DAT - SR),
Razonamiento Abstracto (DAT- AR),
Aptitud Numérica (DAT - NA),
Razonamiento Mecánico (DAT-MR),
Rapidez y precisión perceptiva (DAT -CSA),
Hábitos,
Aprobación,
tipo institución.

Existe una variable llamada "Segunda carrera", la cuál no es relevante, ya que la mayoría de los estudiantes no completan esta parte, y además, se identifico que la mayoría de las observaciones (5200) tienen valor ausente.

Por otro lado las variables: Estado, Estado_actual, CUM y Avance, no son relevantes para la predicción.

Es plausible considerar que las variables 'Carrera' y 'Facultad' pueden ser redundantes, sin embargo, se decidió dejarlas presentes en el desarrollo del modelo, ya que una facultad engloba varias carreras y en algunas carreras se tienen muy pocas observaciones, podría ser relevante dejar ambas.

## Selección de modelo:

Desde la perspectiva técnica, el modelo con mejor desempeño es el Arbol de decisión, sin embargo, es muy probable que se prefiera Random Forest bajo la consideración académica de la influenca que representan las aptitudes en el desempeño estudiantil. Una implementación de este modelo en producción posiblemente requiera un reentrenamiento con una muestra que reduzca la proporción 2:1 actual de la variable objetivo, para que las clases sean mas parejas y el sesgo actual se reduzca.

Es posible que se requiera la aplicación de técnicas de selección de variables, transformación o preparación previas a la construcción del modelo para optimizar aún más los desempeños alcanzados actualmente
