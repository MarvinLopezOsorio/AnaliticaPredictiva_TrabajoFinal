# AnaliticaPredictiva_TrabajoFinal
El estudio se basó en un conjunto de datos generales, encuestas de hábitos de estudio y resultados de análisis psicopedagógicos de los estudiantes del primer ciclo de carreras de ingeniería en una universidad de El Salvador.

# Objetivo
Predecir si un estudiante reprobará el primer ciclo universitario mediante un modelo de clasificación basado en variables psicopedagógicas, conductuales (malos hábitos) y generales.

# El dataset original continene las siguientes variables:

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
