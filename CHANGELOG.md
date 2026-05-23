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
