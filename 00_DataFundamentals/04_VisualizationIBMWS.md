# Limpieza, Refinación y visualización con IBM Watson Studio

IB Watson Studio es un entorno de desarrollo integrado (IDE). Resuelve problemas de desarrollo de IA, ofrece un entorno de aprendizaje automático y ciencia de datos colaborativo y fácil de usar para crear y entrenar modelos, preparar y analizar datos y compartir información en un solo lugar.

IBM Watson Studio ofrece a los científicos de datos:

+ un proceso simplificado para los proyectos de datos
+ un entorno colaborativo de ciencia de datos y aprendizaje automático
+ visualizaciones fáciles de crear
+ acceso a herramientas de código abierto
+ una manera de desarrollar, entrenar, gestionar e implementar aplicaciones impulsadas por IA

## Refinería de datos

La refinería de datos de IBM Watson Studio puede transformar rápidamente grandes cantidades de datos sin procesar en información consumible de gran calidad lista para el análisis.

+ crear un flujo de trabajo para limpiar y dar forma a los datos
+ comprender la calidad y distribución de los datos mediante docenas de gráficos, tablas y estadísticas integrados
+ programar trabajos de datos para resultados repetibles
+ visualizar datos para descubrir información

La herramienta de refinería de datos es interactiva y fácil de utilizar. No necesitas habilidades de codificación. ¡Hay más de 100 operaciones integradas disponibles.

### Pasos de simulación: preparación de proyecto y carga de datos en IBM Watson Studio

1. Abrir IBM Cloud
2. Ir al catalogo
3. En Categoría seleccionar AI/MachineLearning
4. Seleccionar Watson Studio
5. Establecer la ubicación
6. En configuración del servicio establecer el nombre del servicio
7. CREAR
8. Para crear un proyecto seleccionar Launch in IBM Cloud Pak for data
9. En a pestaña projects seleccionar el icono + para generar un nuevo proyecto
10. seleccionar Create Empty Project
11. Establecer el nombre del proyecto
12. Verificar que en Storage se disponga de una base de datos COS (Cloud Object Storage)
13. CREAR
14. Una vez creado el proyecto seleccionar ASSETS (recursos)
15. Para cargar un nuevo conjunto de datos seleccionar NEW ASSET
16. Arrastrar o buscar en el equipo el documento con los datos hacia el espacio DATA in this PROJECT
17. Verificar en la pestaña ALL ASSETS que se ha cargado en archivo, es posible visualizar los datos seleccionando el archivo

### Pasos de Simulación: Comprensión y limpieza de datos

1. Durante la visualización del archivo de datos seleccionar PREPARE DATA
2. La refinería de datos tardara unos mins en leer y procesar los datos
3. Explorar en las pestañas DATA, PROFILE, VISUALIZATION
4. Eliminar las columnas que no son útiles después de verificar los perfiles estadísticos en la pestaña PROFILE. Yendo a la pestaña DATA y eligiendo la opción REMOVE COLUMN es los tres puntos de opciones de la columna.
5. Durante la limpieza ademas de borrar columnas que no son predecibles, con IP o con datos vacíos es necesario verificar los formatos de los datos y que correspondan con los valores observados (INTEGER, DECIMAL, DATETIME, DATE, STRING, etc.).
6. después de haber limpiado completamente seleccionar SAVE AND CREATE A JOB
7. Definir el nombre del trabajo, se puede dejar en blanco la descripción del trabajo
8. Se pueden conservar los valores por defecto que se generaron para los nombre de los archivos de datos FUENTE y los datos LIMPIOS
9. Definir el PROGRAMA (SCHEDULE), mantener apagado o programar que se ejecute a cierta hora si lleva mucho tiempo
10. Definir las notificaciones dependiendo del PROGRAMA
11. Una vez definidas las variables del trabajo seleccionar el botón CRATE AND RUN

### Pasos de simulación: Refinería de datos

1. Ingresar al archivo de datos creado después de la limpieza de datos filename_Shaped.csv. en este nuevo archivo ya no están las columnas que se han eliminado en la limpieza
2. Después de generar una hipótesis sobre los datos, ponerla a prueba.
3. para generar una nueva columna a partir de una ya existente seleccionar los tres puntos de opciones y seleccionar NEW STEP
4. Seleccionar CALCULATE
5. establecer el operador
6. nombrar la nueva columna
7. posicionar la columna
8. si se generan valores booleanos sera mas fácil trabajar con su equivalente entero

### Visualización con IBM Watson Studio

1. en la pestaña VISUALIZATION buscar el tipo de gráfico que sea ideal para representar los datos
2. asignar las variables a los ejes y los mapas de color que sean necesarios
3. las gráficas son dinámicas asi que se pueden inspeccionar los valores mostrados.

## Resumen

1. IBM Watson Studio es un entorno de desarrollo integrado (IDE) que ofrece la herramienta de refinería de datos para limpiar, dar forma y visualizar datos.  

2. El objetivo de tu proyecto de ciencia de datos es predecir el fraude y la actividad sospechosa para ayudar a reducir considerablemente las pérdidas debidas a los fraudes. El fraude es un problema para la compañía de seguros de automóviles.

3. Trabajaste con un conjunto de datos de reclamaciones de seguros de automóviles ficticias con 975 filas y 38 columnas.

4. Tuviste la oportunidad de obtener experiencia práctica en simulaciones de IBM Watson Studio y la herramienta de refinería de datos para:

    1. aprovisionar el servicio de Watson Studio
    2. configurar un nuevo proyecto
    3. importar datos de reclamaciones de seguros de automóviles
    4. limpiar el conjunto de datos
    5. refinar el conjunto de datos
    6. crear y estudiar una visualización de datos para obtener información

5. Has considerado la hipótesis de la patrocinadora empresarial y has sacado conclusiones de la visualización de datos que creaste.
