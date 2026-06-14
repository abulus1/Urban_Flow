# Changelog

## [Sprint 1] - Ejercicio 01
### Agustin Sanchez
- Inicialización del repositorio git
- Creación de la rama Sprint_1
- Creación de la estructura de directorios del proyecto
- Creación de README.md y CHANGELOG.md

## [Sprint 1] - Ejercicio 02
### Agustin Fernandez
- Descarga del dataset raw y almacenamiento en urban_flow/data/raw
- Análisis de tipos de datos y valores nulos

## [Sprint 1] - Ejercicio 03
### Candela Barboza
- Normalización de fechas, horas, ubicaciones y patentes
- Eliminación de filas con valores relevantes vacíos
- Detección y eliminación de outliers
- Creación de columnas exceso_velocidad_real y exceso_velocidad
- Eliminación de filas sin infracción
- Guardado del dataset limpio en urban_flow/data/interim

## [Sprint 1] - Ejercicio 04
## Joaquin Calderon
Implementación de la clase FineAnalyzer
Métodos: ranking_patentes, ranking_horarios, exceso_promedio, exceso_real_promedio, multas_por_ubicacion

## [Sprint 1] - Ejercicio 05
### Agustin Sanchez
- Gráfico de barras horizontal top 10 patentes reincidentes
- Gráfico de torta de infracciones por hora
- Gráfico de barras horizontal de infracciones por mes
- Gráfico de líneas de excesos por hora 00:00
- Gráfico de líneas de excesos por fecha 1932-01-01

## [Sprint 1] - Ejercicio 06
### Agustin Fernandez
- Cálculo del porcentaje de infracciones en fecha 1932-01-01
- Cálculo del porcentaje de infracciones a la hora 00:00

## [Sprint 1] - Ejercicio 07
### Agustin Fernandez
- Redacción de la conclusión del análisis de los datos del dataset

## [Sprint 2] - Ejercicio 01
### Agustin Fernandez
- Inicializacion de la rama Sprint_2 desde Sprint_1
- Descarga y descompresion del dataset de imagenes en urban_flow/data/raw/imgs
- Actualizacion de README.md con contexto del Sprint 2

## [Sprint 2] - Ejercicio 02
### Candela Barboza
- Listado de imagenes con nombre y tamaño en KB
- Clasificacion en grupos plates y completes
- Creacion del diccionario group_images guardado en urban_flow/data/interim
- Implementacion de funcion mostrar_imagenes reutilizable
- Visualizacion de imagenes originales

## [Sprint 2] - Ejercicio 03
### Agustin Sanchez
- Conversion a escala de grises en 03_01_gray_scale/{plates,completes}
- Suavizado GaussianBlur en 03_02_blur/{plates,completes}
- Deteccion de bordes Canny en 03_03_canny/{plates,completes}
- Actualizacion de group_images.json con path_gray, path_blur, path_canny

## [Sprint 2] - Ejercicio 04
### Joaquin Calderon
- Extraccion de patentes via OCR sobre ambos grupos
- Actualizacion de group_images.json con patentes detectadas
- Matching posicional izquierda-derecha con umbral 80%
- Dataset final guardado en urban_flow/data/processed

## [Sprint 2] - Ejercicio 04
### Agustin Fernandez
- Extraccion de patentes via OCR sobre ambos grupos
- Actualizacion de group_images.json con patentes detectadas
- Matching posicional izquierda-derecha con umbral 80%
- Dataset final guardado en urban_flow/data/processed

## [Sprint 2] - Ejercicio 01
### Agustin Fernandez
- Inicializacion de la rama Sprint_2 desde Sprint_1
- Descarga y descompresion del dataset de imagenes en urban_flow/data/raw/imgs
- Actualizacion de README.md con contexto del Sprint 2

## [Sprint 2] - Ejercicio 02
### Candela Barboza
- Listado de imagenes con nombre y tamaño en KB
- Clasificacion en grupos plates y completes
- Creacion del diccionario group_images guardado en urban_flow/data/interim
- Implementacion de funcion mostrar_imagenes reutilizable
- Visualizacion de imagenes originales

## [Sprint 2] - Ejercicio 03
### Agustin Sanchez
- Conversion a escala de grises en 03_01_gray_scale/{plates,completes}
- Suavizado GaussianBlur en 03_02_blur/{plates,completes}
- Deteccion de bordes Canny en 03_03_canny/{plates,completes}
- Actualizacion de group_images.json con path_gray, path_blur, path_canny

## [Sprint 2] - Ejercicio 04
### Agustin Fernandez
- Extraccion de patentes via OCR sobre ambos grupos
- Actualizacion de group_images.json con patentes detectadas
- Matching posicional izquierda-derecha con umbral 80%
- Dataset final guardado en urban_flow/data/processed

## [Sprint 2] - Ejercicio 01
### Agustin Fernandez
- Inicializacion de la rama Sprint_2 desde Sprint_1
- Descarga y descompresion del dataset de imagenes en urban_flow/data/raw/imgs
- Actualizacion de README.md con contexto del Sprint 2

## [Sprint 2] - Ejercicio 02
### Candela Barboza
- Listado de imagenes con nombre y tamaño en KB
- Clasificacion en grupos plates y completes
- Creacion del diccionario group_images guardado en urban_flow/data/interim
- Implementacion de funcion mostrar_imagenes reutilizable
- Visualizacion de imagenes originales

## [Sprint 2] - Ejercicio 03
### Agustin Sanchez
- Conversion a escala de grises en 03_01_gray_scale/{plates,completes}
- Suavizado GaussianBlur en 03_02_blur/{plates,completes}
- Deteccion de bordes Canny en 03_03_canny/{plates,completes}
- Actualizacion de group_images.json con path_gray, path_blur, path_canny

## [Sprint 2] - Ejercicio 04
### Agustin Fernandez
- Extraccion de patentes via OCR sobre ambos grupos
- Actualizacion de group_images.json con patentes detectadas
- Matching posicional izquierda-derecha con umbral 80%
- Dataset final guardado en urban_flow/data/processed

## [Sprint 2] - Ejercicio 05 y 06
### Joaquin Calderon
- Calculo de metricas finales del dataset procesado.
- Analisis de multas con y sin imagenes asociadas.
- Identificacion de imagenes sin coincidencia dentro del dataset.
- Analisis de multas pendientes de pago con soporte visual relacionado.
- Incorporacion de conclusiones generales del Sprint 2.
- Documentacion del flujo OCR y matching de patentes.
- Descripcion de limitaciones del reconocimiento automatico de caracteres.

## [Sprint 2] - Ejercicio 01
### Agustin Fernandez
- Inicializacion de la rama Sprint_2 desde Sprint_1
- Descarga y descompresion del dataset de imagenes en urban_flow/data/raw/imgs
- Actualizacion de README.md con contexto del Sprint 2

## [Sprint 2] - Ejercicio 02
### Candela Barboza
- Listado de imagenes con nombre y tamaño en KB
- Clasificacion en grupos plates y completes
- Creacion del diccionario group_images guardado en urban_flow/data/interim
- Implementacion de funcion mostrar_imagenes reutilizable
- Visualizacion de imagenes originales

## [Sprint 2] - Ejercicio 03
### Agustin Sanchez
- Conversion a escala de grises en 03_01_gray_scale/{plates,completes}
- Suavizado GaussianBlur en 03_02_blur/{plates,completes}
- Deteccion de bordes Canny en 03_03_canny/{plates,completes}
- Actualizacion de group_images.json con path_gray, path_blur, path_canny

## [Sprint 2] - Ejercicio 04
### Agustin Fernandez
- Extraccion de patentes via OCR sobre ambos grupos
- Actualizacion de group_images.json con patentes detectadas
- Matching posicional izquierda-derecha con umbral 80%
- Dataset final guardado en urban_flow/data/processed

## [Sprint 2] - Ejercicio 05 y 06
### Joaquin Calderon
- Calculo de metricas finales del dataset procesado.
- Analisis de multas con y sin imagenes asociadas.
- Identificacion de imagenes sin coincidencia dentro del dataset.
- Analisis de multas pendientes de pago con soporte visual relacionado.
- Incorporacion de conclusiones generales del Sprint 2.
- Documentacion del flujo OCR y matching de patentes.
- Descripcion de limitaciones del reconocimiento automatico de caracteres.

## [Sprint 3] - Ejercicio 01
### Agustin Sanchez
- Inicialización de la rama Sprint_3 desde Sprint_2
- Verificación de acceso a todos los datasets generados
- Actualización de README.md con contexto del Sprint 3

## [Sprint 3] - Ejercicio 02
### Agustin Fernandez
Inicializacion de DVC y configuracion de remote local
Migracion del directorio de imagenes urban_flow_plates a DVC
Migracion del archivo speeding_fines_image.csv a DVC

## [Sprint 3] - Ejercicio 03
### Agustin Fernandez
Diseño del modelo logico con clases Vehiculo, Radar, Evidencia y Multa
Definicion de relaciones entre entidades

## [Sprint 3] - Ejercicio 04
### Agustin Sanchez
- Implementacion de la funcion procesar_fila_csv
- Mapeo de diccionario CSV a instancias del modelo logico
- Manejo de evidencia opcional segun disponibilidad de imagen

## [Sprint 3] - Ejercicio 05
### Agustin Fernandez
- Diseño del modelo relacional con SQLAlchemy ORM
- Definicion de claves primarias y foreign keys entre tablas
- Implementacion de relaciones ORM (Vehiculo, Radar, Evidencia, Multa)
- Sobrescritura de __repr__ en cada modelo para mejor legibilidad

## [Sprint 3] - Ejercicio 01
### Agustin Sanchez
- Inicialización de la rama Sprint_3 desde Sprint_2
- Verificación de acceso a todos los datasets generados
- Actualización de README.md con contexto del Sprint 3

[Sprint 3] - Ejercicio 02
Agustin Fernandez
Inicializacion de DVC y configuracion de remote local
Migracion del directorio de imagenes urban_flow_plates a DVC
Migracion del archivo speeding_fines_image.csv a DVC

[Sprint 3] - Ejercicio 03
Agustin Fernandez
Diseño del modelo logico con clases Vehiculo, Radar, Evidencia y Multa
Definicion de relaciones entre entidades

## [Sprint 3] - Ejercicio 04
### Agustin Sanchez
- Implementacion de la funcion procesar_fila_csv
- Mapeo de diccionario CSV a instancias del modelo logico
- Manejo de evidencia opcional segun disponibilidad de imagen

## [Sprint 3] - Ejercicio 05
### Agustin Fernandez
- Diseño del modelo relacional con SQLAlchemy ORM
- Definicion de claves primarias y foreign keys entre tablas
- Implementacion de relaciones ORM (Vehiculo, Radar, Evidencia, Multa)
- Sobrescritura de __repr__ en cada modelo para mejor legibilidad

## [Sprint 3] - Ejercicio 06
### Agustin Sanchez
- Creacion de la base de datos transito con SQLAlchemy
- Creacion automatica de tablas desde el modelo ORM
- Migracion de datos desde speeding_fines_image.csv
- Validacion de cantidad de registros insertados

## [Sprint 3] - Ejercicio 01
### Agustin Sanchez
- Inicialización de la rama Sprint_3 desde Sprint_2
- Verificación de acceso a todos los datasets generados
- Actualización de README.md con contexto del Sprint 3

[Sprint 3] - Ejercicio 02
Agustin Fernandez
Inicializacion de DVC y configuracion de remote local
Migracion del directorio de imagenes urban_flow_plates a DVC
Migracion del archivo speeding_fines_image.csv a DVC

[Sprint 3] - Ejercicio 03
Agustin Fernandez
Diseño del modelo logico con clases Vehiculo, Radar, Evidencia y Multa
Definicion de relaciones entre entidades
