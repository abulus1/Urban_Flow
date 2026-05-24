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
