
## Objetivo general:

Analizar el sentimiento en el lenguaje de los políticos para averiguar si éste influye en su popularidad. 

## Objetivos específicos

Descubrir cuál es el sentimiento principal que se desprende de cada texto por persona, partido y fecha
Construir un conjunto de datos propio para los fines del proyecto
Aplicar ciertas funciones propias del lenguaje natural (NLP) de los textos 
Analizar las palabras más frecuentes y el sentimiento que revela cada texto en su conjunto
Comparar estadísticamente y relacionar los datos, en tiempo y en cantidad con la evolucón de estas personas y de las formaciones políticas que representan a nivel municipal

## Presentación del conjunto de datos

Se toman los textos de los regidores y regidoras que representan las principales formaciones políticas y también los de los alcaldes
que hubo entre 2012 y 2023 en Sant Boi de Llobregat, un municipio del Área Metropolitana de Barcelona de unos 85 mil 
habitantes. Estos textos son descargados desde su versión en línea del periódico municipal “Viure Sant Boi”. A parte de encontrarse 
en internet a través de la web del ayuntamiento, dicho informativo es distribuido a principios de cada mes a todos los hogares de 
Sant Boi de Llobregat a través de correos, en formato papel. Los textos tienen el formato de cartas de opinión que se dirigen a los 
ciudadanos, donde cada regidor así como la alcaldesa o el alcalde en funciones, comunican y sus pensamientos sobre temas de 
actualidad, o sobre programas, hechos y decisiones públicas que impactan directamente la gente del municipio. De los regidores y 
regidoras, uno representa el partido en el poder y los demás representan a la oposición.   

## El conjunto de datos tiene las siguientes variables:

  RangeIndex: 134 entries, 0 to 133
  
  Data columns (total 17 columns):
  
   ###   Column                  Non-Null Count  Dtype  
   
  ---  ------                  --------------  -----  
   0   Fecha                   134 non-null    object 
   
   1   Año                     134 non-null    object 
   
   2   Mes                     134 non-null    object 
   
   3   Temas portada           134 non-null    object 
   
   4   Temas portada en        134 non-null    object 
   
   5   Partido                 134 non-null    object 
   
   6   Persona                 134 non-null    object 
   
   7   Original                134 non-null    object 
   
   8   Traducción              134 non-null    object 
   
   9   Codigo_id               134 non-null    object 
   
   10  Negative                134 non-null    float64
   
   11  Neutral                 134 non-null    float64
   
   12  Positive                134 non-null    float64
      
   13  Compound                134 non-null    float64
   
   14  Avg_Positive_Sentences  134 non-null    float64
   
   15  Avg_Negative_Sentences  134 non-null    float64
   
   16  Avg_Neutral_Sentences   134 non-null    float64
   
  dtypes: float64(7), object(10)


Fuente de los datos: descargados desde su versión en línea del periódico mensual “Viure Sant Boi”. Conjunto de datos de 
elaboración propia

Los datos cubren 2 años de publicaciones en el "Viure Sant Boi", repartidos en 20 fechas (se publica 10 meses al año ya que enero y febrero van juntos, como también julio y agosto)
Hay 9 entidades de “partido”, de los cuales 1 es la alcaldía, que intervine a cada publicación, a diferencia de los regidores de su partido, que se alternan.
Se recopilaron los textos de 27 personas políticas, entre las cuales, la alcaldesa de Sant Boi de Llobregat durante el periodo estudado

Con todo, son 134 los textos de opinión recopilados que han escrito a los ciudadanos, cada uno en lengua original y su traducción al inglés como variables separada

## Metodología, procesos y herramientas:
 Los textos serán los originales en catalán o castellano y se guardarán por fecha, por persona y partido, para formar un 
conjunto de datos temporal mensual sobre varios años.
 Muchas herramientas de NLP funcionan mejor con el idioma inglés, por lo que cada texto se traducirá y se revisará, aparte 
de mantener el original en una columna aparte. 
 Se hará el EDA (estudio descriptivo y analítico del conjunto de datos)
 Se procederá a algunas transformaciones del conjunto de datos inicial
 Se usarán algoritmos para conocer las palabras y conceptos más utilizados en sus comunicaciones con los ciudadanos
 Tras conocer las palabras más usadas por persona y mes, se procederá al análisis de sentimiento para resaltar polaridades 
(positivo, negativo, neutro, etc.)

* La popularidad se entiende por los resultados en las elecciones 
* El lenguaje de programación para este trabajo será Python y las librerías de análisis y procesamiento de texto Nltk, Spacy, 
Stanza, así como Pandas, Seaborn y Matplotlib para tablas y gráficos.


