# Urban Flow

## Sprint 1

### Objetivo
Aplicar conocimientos de versionado, organización y limpieza de código utilizando pandas para depurar datos históricos de multas por exceso de velocidad.

### Introducción y Contexto
La localidad de Vaalserberg (Bélgica), ubicada en zona fronteriza con Países Bajos y Alemania, cuenta con un sistema de radares urbanos para detección de infracciones por exceso de velocidad. Los registros históricos provienen de sistemas heredados con errores de formato y datos faltantes. El objetivo es analizar y depurar estos datos para incorporarlos al nuevo sistema sin inconsistencias.
## Conclusión del Análisis

El dataset original contenía valores nulos significativos: **1957 registros** sin velocidad registrada, **1002** sin `radar_id` y **50** sin patente.
Las columnas `fecha` y `hora` presentaron múltiples formatos inconsistentes que fueron normalizados a un estándar único durante la limpieza. Como resultado de este proceso, se eliminaron **1982 filas** que no cumplían con los criterios mínimos de calidad. No se detectaron outliers en las columnas numéricas analizadas (`velocidad_registrada`, `velocidad_maxima`, `patente`).

### Anomalías detectadas

El análisis temporal reveló dos anomalías críticas que distorsionan los resultados:

- El **26.44%** de las infracciones están registradas en la fecha `1932-01-01`.
- El **19.79%** de las infracciones están registradas a las `00:00hs`. Se mezclan registros con hora inválida normalizada a `00:00` junto con infracciones reales ocurridas a medianoche, lo que imposibilita distinguir ambos casos.

**Enero** aparece como el mes con más infracciones con una diferencia de casi **400 registros** sobre diciembre, comportándose como un outlier mensual. Esto es consistente con la contaminación de la fecha `1932-01-01`, cuyos registros al ser mal parseados pudieron haber caído en enero.

### Consideraciones finales

Los resultados del análisis temporal deben interpretarse con cautela, dado que aproximadamente el **46% de los registros** presentan anomalías en fecha u hora.

Sugerimos analizar mejor las validaciones en origen y definir un criterio claro para el tratamiento de registros con fecha y hora inválidas, estableciendo que aquellos que no puedan ser interpretados sean marcados como **vacíos** en lugar de asignarles valores por defecto, evitando así que distorsionen el análisis.

  ---
## Sprint 2

### Objetivo
Aplicar conocimientos de tratamiento de imagenes y programacion limpia
para determinar que multas tienen evidencia visual valida.

### Introduccion y Contexto
Los radares urbanos generan registros de multas automaticamente y las
camaras asociadas registran la evidencia visual. No todas las multas
tienen imagen asociada, no todas las imagenes corresponden a una
infraccion y puede haber errores de deteccion. El objetivo es
determinar que multas tienen evidencia visual valida.

  ---
## Sprint 2

### Objetivo
Aplicar conocimientos de tratamiento de imagenes y programacion limpia
para determinar que multas tienen evidencia visual valida.

### Introduccion y Contexto
Los radares urbanos generan registros de multas automaticamente y las
camaras asociadas registran la evidencia visual. No todas las multas
tienen imagen asociada, no todas las imagenes corresponden a una
infraccion y puede haber errores de deteccion. El objetivo es
determinar que multas tienen evidencia visual valida.

  ---
## Sprint 2

### Objetivo
Aplicar conocimientos de tratamiento de imagenes y programacion limpia
para determinar que multas tienen evidencia visual valida.

### Introduccion y Contexto
Los radares urbanos generan registros de multas automaticamente y las
camaras asociadas registran la evidencia visual. No todas las multas
tienen imagen asociada, no todas las imagenes corresponden a una
infraccion y puede haber errores de deteccion. El objetivo es
determinar que multas tienen evidencia visual valida.

# Sprint 2 - Ejercicio 06: Conclusiones finales

En este segundo sprint se incorporó el procesamiento de imágenes al análisis de multas trabajado previamente. El objetivo principal fue relacionar el dataset tabular de infracciones con evidencia visual asociada a cada registro.

Durante el desarrollo se clasificaron las imágenes disponibles entre fotografías completas y recortes de patentes. Luego se aplicaron técnicas básicas de procesamiento de imágenes, como conversión a escala de grises, suavizado con Gaussian Blur y detección de bordes mediante Canny.

Posteriormente se utilizó OCR para extraer automáticamente posibles patentes desde las imágenes. Estas patentes fueron comparadas con las patentes del dataset final mediante un criterio de similitud, permitiendo identificar coincidencias aproximadas entre registros e imágenes.

A partir de las métricas calculadas en el Ejercicio 05, se pudo obtener una visión general sobre la cantidad de multas con imágenes asociadas, multas sin evidencia visual, imágenes sin coincidencia y multas pendientes con imagen relacionada.

Como limitación principal, el reconocimiento OCR puede fallar cuando las imágenes presentan baja resolución, mala iluminación, inclinación, ruido visual o patentes parcialmente visibles. Por este motivo, los resultados deben interpretarse como una aproximación inicial y no como una validación definitiva.

En conclusión, el sprint permitió integrar datos estructurados e imágenes dentro de un mismo flujo de trabajo, fortaleciendo el análisis de multas mediante evidencia visual y dejando una base preparada para mejoras futuras en la detección automática de patentes.

  ---
## Sprint 2

### Objetivo
Aplicar conocimientos de tratamiento de imagenes y programacion limpia
para determinar que multas tienen evidencia visual valida.

### Introduccion y Contexto
Los radares urbanos generan registros de multas automaticamente y las
camaras asociadas registran la evidencia visual. No todas las multas
tienen imagen asociada, no todas las imagenes corresponden a una
infraccion y puede haber errores de deteccion. El objetivo es
determinar que multas tienen evidencia visual valida.

# Sprint 2 - Ejercicio 06: Conclusiones finales

En este segundo sprint se incorporó el procesamiento de imágenes al análisis de multas trabajado previamente. El objetivo principal fue relacionar el dataset tabular de infracciones con evidencia visual asociada a cada registro.

Durante el desarrollo se clasificaron las imágenes disponibles entre fotografías completas y recortes de patentes. Luego se aplicaron técnicas básicas de procesamiento de imágenes, como conversión a escala de grises, suavizado con Gaussian Blur y detección de bordes mediante Canny.

Posteriormente se utilizó OCR para extraer automáticamente posibles patentes desde las imágenes. Estas patentes fueron comparadas con las patentes del dataset final mediante un criterio de similitud, permitiendo identificar coincidencias aproximadas entre registros e imágenes.

A partir de las métricas calculadas en el Ejercicio 05, se pudo obtener una visión general sobre la cantidad de multas con imágenes asociadas, multas sin evidencia visual, imágenes sin coincidencia y multas pendientes con imagen relacionada.

Como limitación principal, el reconocimiento OCR puede fallar cuando las imágenes presentan baja resolución, mala iluminación, inclinación, ruido visual o patentes parcialmente visibles. Por este motivo, los resultados deben interpretarse como una aproximación inicial y no como una validación definitiva.

En conclusión, el sprint permitió integrar datos estructurados e imágenes dentro de un mismo flujo de trabajo, fortaleciendo el análisis de multas mediante evidencia visual y dejando una base preparada para mejoras futuras en la detección automática de patentes.

---
## Sprint 3

### Objetivo
Profesionalizar la solución incorporando persistencia en base de datos
relacional mediante SQLAlchemy, control de versiones de datos con DVC
y preparación para búsquedas avanzadas con ChromaDB.

### Introducción y Contexto
El sistema ha crecido en volumen de datos y complejidad, por lo que ya
no es viable trabajar únicamente con archivos CSV. En este Sprint se
migra la información procesada a una base de datos estructurada,
se versiona con DVC y se incorpora una base de datos vectorial.
