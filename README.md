# 📊Analítica de Datos - Intro. Ing. de Sistemas

[Go to .ipynb File](https://colab.research.google.com/assets/colab-badge.svg)

## 👥Integrantes
- Catalina Forero
- Maria Sierra
- Rafael Sierra
#

## 📝Introducción

### Contexto
El presente análisis se basa en el conjunto de datos publicado por el Gobierno de Colombia sobre el volumen de solicitudes de visa colombiana recibidas. Este dataset contiene información detallada de los solicitantes, incluyendo su nacionalidad, sexo, año de solicitud y tipo de visa. El objetivo es identificar tendencias y patrones en las solicitudes, facilitando una comprensión general del perfil de los solicitantes y su distribución a lo largo del tiempo.

### Justificación del Análisis
Este análisis de datos sobre las solicitudes de visa para Colombia es útil para diferentes personas e instituciones que necesitan entender cómo se mueve la migración en el país. Para el Departamento de Migración, la información ayuda a saber de qué países vienen más solicitantes y si hay diferencia entre hombres y mujeres que solicitan visa. Esto les sirve para tomar decisiones sobre políticas migratorias y controlar mejor las entradas al país.

También es importante para las empresas que buscan contratar extranjeros, ya que con estos datos pueden saber en qué años han aumentado las solicitudes de visa con intención de quedarse en Colombia y cuál es la edad promedio de esas personas. Así, pueden planear mejor sus procesos de contratación.

Además, los datos pueden ser útiles para periodistas o medios de comunicación, porque les permite informar cuántas solicitudes de visa se han hecho cada año desde 2017 y qué porcentaje representan las diferentes nacionalidades. Esto ayuda a que las personas entiendan mejor qué está pasando con la migración en Colombia.

#

## 🛠️Metodología

### Datos Generales del Data Set
- **Nombre del dataset:** Volumen de Solicitudes de Visa Colombiana recibidas desde 2017
- **Datos suministrados por:** Ministerio de Relaciones Exteriores
- **Categoría:** Estadísticas Nacionales
- **Idioma:** Español
- **Cobertura Geográfica:** Internacional
- **Fecha de creación:** 26 de diciembre del 2024
- **Última actualización:** 26 de diciembre del 2024
- **Número de filas:** 350k
- **Número de columnas:** 6
- **Cada fila es:** una solicitud de visa
- **Datos que contiene:** Contiene información sobre el número anual de solicitudes de visas recibidas por parte de la Autoridad de Visas e Inmigración, fecha de solicitud, sexo, nacionalidad, fecha de nacimiento del solicitante y la vocación de permanencia.

| Nombre de la Columna        | Descripción                                       | Tipo de Dato             |
| --------------------------- | ------------------------------------------------- | ------------------------ |
| **Año Solicitud**           | Año en el que se radica la solicitud              | Número                   |
| **Nacionalidad**            | Nacionalidad registrada en el pasaporte           | Texto                    |
| **Sexo**                    | Sexo registrado por el solicitante                | Texto                    |
| **Fecha de Nacimiento**     | Fecha de nacimiento registrada por el solicitante | Marca de tiempo variable |
| **Vocación de Permanencia** | Tipo de visa solicitada                           | Texto                    |
| **Número**                  | Número de visas                                   | Número                   |
#

### 👤Perfiles

**`Hacer clic en el perfil que desea revisar los resultados para dirigirse a las respuestas de las preguntas y sus respectivas gráficas`**

#### [**🔗 Perfil #1 - Departamento de Migración (Política migratoria y control fronterizo)**](/1-Perfil/README.md)

Este perfil corresponde a académicos, analistas o funcionarios que estudian tendencias migratorias.

- **Pregunta #1** - ¿Cuáles son los países con más solicitantes de visa para Colombia?
- **Pregunta #2** - ¿Existe una diferencia significativa en la cantidad de solicitudes según el sexo del solicitante?

#### [**🔗 Perfil #2 - Reclutador de Talento Internacional**](/2-Perfil/README.md)

Empresas que buscan contratar talento extranjero o gestionar movilidad laboral.

- **Pregunta #1** - ¿Cuáles son los años con mayor crecimiento en solicitudes de visa con vocación de permanencia? 
- **Pregunta #2** - ¿Qué edad promedio tienen los solicitantes de visa con vocación de permanencia?

#### [**🔗 Perfil #3 - Periodista en Medios de Comunicación**](/3-Perfil/README.md)

Interesado en informar sobre tendencias migratorias en Colombia.

- **Pregunta #1** - ¿Cuántas solicitudes de visa se han registrado anualmente en Colombia desde el 2017? 
- **Pregunta #2** - ¿Qué porcentaje del total de solicitudes corresponde a cada nacionalidad?
#

### 🧰Herramientas Utilizadas en el Análisis
Para realizar este análisis de datos, se utilizó el lenguaje de programación **Python**, junto con las librerías **Pandas**, **Matplotlib** y **Seaborn**, que permitieron organizar, procesar y visualizar la información del dataset.

Con **Pandas** se hizo la carga y limpieza de los datos, además de los cálculos estadísticos como el **promedio**, **conteo** y **porcentaje** de las solicitudes de visa, según variables como nacionalidad, sexo y año de solicitud.

Para la visualización de los resultados, se usaron gráficos elaborados con **Matplotlib** y **Seaborn**, específicamente:

- **Gráficos de barras.** Para mostrar la cantidad de solicitudes por sexo y por año.

- **Gráfico de pastel (pie chart).** Para representar los porcentajes de solicitudes por nacionalidad.

- **Gráficos de línea.** Para mostrar la evolución anual de las solicitudes.

Estas herramientas permitieron identificar patrones, diferencias y tendencias en las solicitudes de visa colombiana registradas en los últimos años.
#

## ✅Resultados

Los resultados se encuentran en cada carpeta de cada perfil con su respectiva grafica y explicación. Cada carpeta tiene un archivo README que tiene las respuestas y a su vez las graficas.
#

## 📌Conclusiones
1. Venezuela es el país con mayor cantidad de solicitantes de visa para Colombia, seguido por otros países como Estados Unidos, Cuba y España, lo que refleja una tendencia migratoria.

1. Existe una diferencia significativa en las solicitudes según el sexo: la mayoría de las solicitudes fueron realizadas por personas del sexo masculino, aunque esto puede deberse a varios factores sociales o familiares.

2. El número de solicitudes de visa aumentó notablemente en el año 2018, con un incremento significativo, mientras que en otros años hubo un decremento en solicitudes de visa lo que puede relacionarse con crisis sociales, políticas o económicas en algunos países.

3. La mayoría de las solicitudes de visa con vocación de permanencia provienen de personas con un rango de edad entre 25 y 40 años, lo que indica un perfil joven y productivo que busca establecerse en Colombia.

4. El promedio de edad de los solicitantes de visa con vocación de permanencia es de aproximadamente 35 años.

6. A pesar de la alta cantidad de nacionalidades registradas, el 80% de las solicitudes corresponde a un grupo reducido de países, mientras que el resto tiene un porcentaje muy bajo.

7. En los últimos años analizados, se observa una tendencia creciente en el interés de personas extranjeras por establecerse en Colombia, lo que puede tener un impacto en el mercado laboral, la economía y la cultura.

8. Hay una gran diferencia entre la cantidad de solicitudes por sexo, la distribución muestra que el género masculino tienen más participación en la solicitud de visas que el género femenino.

9. El análisis anual revela que los años entre 2018 y 2019 fueron los que registraron el mayor número de solicitudes, posiblemente relacionados con coyunturas migratorias específicas.

10. El análisis muestra que la mayoría de las solicitudes de visa provienen de un grupo reducido de países, lo que evidencia que la migración hacia Colombia está concentrada principalmente en ciertas nacionalidades y no distribuida de manera uniforme entre todos los países.
#

## 🎯Sugerencias para los perfiles
### Para el Departamento de Migración:

- Utilizar estos datos para reforzar la política migratoria con enfoque en los países con mayor número de solicitantes.

- Tener en cuenta las diferencias por sexo y edad para diseñar programas de integración y asistencia específicos.
#

### Para reclutadores de talento internacional:

- Poner atención en el perfil de los solicitantes con vocación de permanencia, ya que la mayoría está en edad productiva.

- Aprovechar el aumento de solicitudes en ciertos países para identificar oportunidades de contratación de talento extranjero.

- Diseñar estrategias para retener y facilitar la inserción laboral de personas que buscan establecerse en Colombia.
#

### Para periodistas y medios de comunicación:

- Utilizar los datos para informar sobre las tendencias migratorias actuales y sus posibles causas.

- Promover la discusión pública sobre los efectos de la migración en Colombia, basándose en datos concretos.

- Generar contenido sobre la diversidad de nacionalidades y la presencia creciente de extranjeros en el país.
#