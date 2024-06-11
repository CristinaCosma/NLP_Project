
## Objetivo general:

Analizar el sentimiento en el lenguaje de los políticos para averiguar si éste influye en su popularidad. 

## Objetivos específicos

Descubrir cuál es el sentimiento principal que se desprende de cada texto por persona, partido y fecha
Construir un conjunto de datos propio para los fines del proyecto
Aplicar ciertas funciones propias del lenguaje natural (NLP) de los textos 
Analizar las palabras más frecuentes y el sentimiento que revela cada texto en su conjunto
Comparar estadísticamente y relacionar los datos, en tiempo y en cantidad con la evolucón de estas personas y de las formaciones políticas que representan a nivel municipal

## El conjunto de datos tiene las siguientes variables:

  RangeIndex: 134 entries, 0 to 133
  
  Data columns (total 17 columns):
  
   #   Column                  Non-Null Count  Dtype  
   
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


cubre 2 años de publicaciones del Viure Sant Boi, 
en 20 fechas (se publica 10 meses al año ya que enero y febrero van juntos, como también julio y agosto)
Hay 9 entidades “partido”, de los cuales 1 es la alcaldía
Se recopilaron los textos de 27 personas políticas, entre las cuales, la alcaldesa

Con todo esto, son 134 los textos de opinión recopilados que han escrito a los ciudadanos, cada uno en lengua original y su traducción al inglés como variables separada

