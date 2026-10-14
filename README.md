# AWS Machine Learning — Labs 3.4 y 3.5

Repositorio académico que documenta el entrenamiento, despliegue y evaluación de un modelo de Machine Learning utilizando Amazon SageMaker y XGBoost.

## Objetivos

- Preparar y transformar datos para entrenar un modelo.
- Dividir los datos en conjuntos de entrenamiento, validación y prueba.
- Almacenar los datos de entrenamiento en Amazon S3.
- Entrenar un modelo XGBoost utilizando Amazon SageMaker.
- Desplegar el modelo para realizar inferencias en tiempo real.
- Ejecutar inferencias por lotes mediante SageMaker Batch Transform.
- Examinar los resultados obtenidos durante la ejecución.
- Gestionar los recursos de AWS utilizados durante la implementación.

## Laboratorio 3.4 — Formación de un modelo

El notebook `3_4-machinelearning.ipynb` documenta el proceso de preparación de los datos y entrenamiento del modelo.

Las actividades incluyen:

- Instalación y utilización de bibliotecas de Python para el procesamiento de datos.
- Lectura y transformación del conjunto de datos en formato ARFF.
- Preparación de las variables y transformación de las etiquetas de clase.
- División de los datos en conjuntos de entrenamiento, validación y prueba.
- Carga de los datos de entrenamiento a Amazon S3.
- Configuración de los hiperparámetros de XGBoost.
- Entrenamiento del modelo mediante Amazon SageMaker.

## Laboratorio 3.5 — Implementación de un modelo

El notebook `3_5-machinelearning.ipynb` documenta la implementación del modelo y la ejecución de inferencias.

Las actividades incluyen:

- Configuración y despliegue del modelo en un endpoint de Amazon SageMaker.
- Preparación de los datos de prueba.
- Ejecución de predicciones individuales mediante el endpoint.
- Preparación de archivos de entrada para inferencia por lotes.
- Ejecución de un trabajo de SageMaker Batch Transform.
- Recuperación y análisis de los resultados de las predicciones.
- Conversión de las puntuaciones obtenidas en etiquetas de clase mediante la lógica implementada en el notebook.
- Eliminación del endpoint de inferencia en tiempo real al finalizar su uso.

## Conjunto de datos

El repositorio incluye archivos relacionados con el conjunto de datos de columna vertebral (Vertebral Column Data Set), utilizado para ejercicios de clasificación.

Archivos incluidos:

- `column_2C.dat`
- `column_2C_weka.arff`
- `column_3C.dat`
- `column_3C_weka.arff`

El archivo `column_2C_weka.arff` se utiliza en el flujo de preparación de datos del laboratorio 3.4. El conjunto de datos contiene características numéricas relacionadas con la columna vertebral y etiquetas de clasificación.

## Tecnologías y herramientas

- Amazon SageMaker: entrenamiento, despliegue e inferencia de modelos de Machine Learning.
- Amazon S3: almacenamiento de datos y archivos utilizados en el entrenamiento y la inferencia.
- XGBoost: algoritmo de aprendizaje automático utilizado para la clasificación.
- Python: lenguaje de programación empleado para desarrollar los ejercicios.
- Jupyter Notebook: entorno interactivo para ejecutar código, documentar procedimientos y examinar resultados.
- Pandas: manipulación y análisis de datos tabulares.
- NumPy: operaciones numéricas.
- SciPy: lectura y procesamiento de datos en formato ARFF.
- Scikit-learn: preparación de conjuntos de datos y otras tareas de aprendizaje automático.
- Boto3: interacción programática con servicios de AWS.

## Estructura del repositorio

    AWS-Lab-3.4-3.5/
    ├── 3_4-machinelearning.ipynb
    ├── 3_5-machinelearning.ipynb
    ├── column_2C.dat
    ├── column_2C_weka.arff
    ├── column_3C.dat
    ├── column_3C_weka.arff
    ├── .gitignore
    └── README.md

## Flujo de trabajo

El proceso desarrollado en los laboratorios se resume en las siguientes etapas:

1. Preparación de los datos: lectura, transformación y organización de las características y etiquetas.
2. División del conjunto de datos: separación de los datos en conjuntos de entrenamiento, validación y prueba.
3. Almacenamiento: carga de los archivos necesarios a Amazon S3.
4. Entrenamiento: configuración y ejecución de XGBoost mediante Amazon SageMaker.
5. Despliegue: creación de un endpoint para realizar inferencias individuales.
6. Inferencia por lotes: procesamiento de múltiples registros mediante SageMaker Batch Transform.
7. Evaluación de resultados: consulta y análisis de las puntuaciones y etiquetas producidas por el modelo.
8. Limpieza de recursos: eliminación de los recursos temporales que ya no sean necesarios.

## Requisitos y consideraciones

Los notebooks están diseñados para ejecutarse en un entorno compatible con Amazon SageMaker y con los permisos necesarios para utilizar los servicios de AWS involucrados.

Para reproducir las prácticas, se deben considerar los siguientes requisitos:

- Acceso a un entorno de Amazon SageMaker.
- Permisos de acceso al bucket de Amazon S3 correspondiente.
- Configuración válida de credenciales y permisos de AWS.
- Disponibilidad de las bibliotecas de Python requeridas.
- Configuración compatible de los hiperparámetros y del contenedor de XGBoost utilizado por SageMaker.

Los nombres de los buckets, las rutas de almacenamiento y otros parámetros pueden variar según el entorno institucional de AWS Academy. Por esta razón, los notebooks pueden requerir ajustes antes de ejecutarse en una cuenta diferente.

Consideración sobre costos: los endpoints de inferencia y otros recursos de AWS pueden generar cargos mientras permanezcan activos. Se recomienda verificar su estado y eliminar los recursos temporales una vez finalizadas las pruebas.

## Evidencias y resultados

Los notebooks contienen el código ejecutado y las salidas que quedaron guardadas durante las prácticas. Entre los resultados documentados se encuentran la preparación de los datos, la creación del modelo, las predicciones individuales y los resultados de inferencia por lotes.

Las capturas de pantalla adicionales se incorporarán si son requeridas por las instrucciones académicas.

## Propósito académico

Este repositorio reúne las actividades prácticas de formación en Machine Learning e implementación de modelos mediante servicios administrados de AWS.

El trabajo permite aplicar conceptos de preparación de datos, entrenamiento supervisado, despliegue de modelos, inferencia en tiempo real y procesamiento por lotes, así como familiarizarse con el ciclo de trabajo de un modelo de aprendizaje automático en un entorno de nube.

---

Autor: Juan Pablo Sánchez Nieto

Repositorio: https://github.com/JPablo1235/AWS-Lab-3.4-3.5

Rama de trabajo: dev_juasanchez35
