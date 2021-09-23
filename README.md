
<p align="center"> 
<img src="https://user-images.githubusercontent.com/69567089/132707858-021aeaf4-8cf9-44e9-b4d3-0350b60418de.png">
</p> 


# Índice
1. [Conceptos generales del Chatbot (Bix) para consultar variables del Mercado de Energía Mayorista](#section1)
2. [Variables disponibles para consultarle a Bix](#section2)
3. [Operaciones aritméticas que pueden realizarse](#section3)
4. [Manejo de fechas relativas](#section4)
5. [Manejo de fechas relativas](#section5)
6. [Ejemplos de uso](#section6)


<p align="center"> 
<img src="https://user-images.githubusercontent.com/69567089/134450647-54c1e086-7069-4b6f-8cb3-8e79018fb882.png">
</p> 

# Conceptos generales del Chatbot (_Bix_) para consultar variables del Mercado de Energía Mayorista
Este repositorio se crea con el objetivo de presentar la documentación de uso para la interfaz conversacional creada por el Equipo de Analítica para consultar las principales variables del Mercado de Energía Mayorista y así facilitar el análisis ejecutivo de información específica. El chatbot recibe el nombre de _Bix_ y llega a hacer complementar del abanico de soluciones que tiene disponible XM para mantener actualizados a los diferentes públicos de interés. 

_Bix_ es un chatbot de tipo _basado en reglas_ por lo cual tiene la capacidad de seguir una serie de reglas y comprender palabras claves o frases típicas para responder preguntas sobre la evolución de variables del Mercado de Energía Mayorista. También, mediante el reconocimiento del texto de la conversación, _Bix_ se encuentra en capacidad de realizar operaciones básicas que detallaremos más adelante en esta documentación.

Dentro de las principales funciones en las que _Bix_ puede asistir son:

* Extracción información de una variable del Mercado de Energía Mayorista mediante el uso del lenguaje natural.
* Exportación de los datos consultados a archivos de Excel.
* Generación de gráficas para facilitar análisis a partir del resultado obtenido.

La interacción con el chatbot pueden ser indicadas utilizando lenguaje natural o señalando los comandos que van surgiendo en la pantalla a medida que se desarrolla la conversación.

Es importante resaltar que el idioma oficial de _Bix_ es el Español.

# Operaciones aritméticas que pueden realizarse

Además de entregar datos extraidos desde las bases de datos de XM a traves de la [API XM](https://github.com/EquipoAnaliticaXM/API_XM), _Bix_ tiene la capacidad de realizar las siguientes operaciones:

* Máximo: Retorna el valor máximo para el periodo de tiempo consultado
* Mínimo: Retorna el valor mínimo para el periodo de tiempo consultado
* Promedio: Retorna el promedio aritmético para el periodo de tiempo consultado
* Máximo diario: Retorna el valor máximo observado para cada día dentro del periodo de tiempo consultado
* Mínimo diario: Retorna el valor mínimo observado para cada día dentro del periodo de tiempo consultado
* Promedio Ponderado diario: Aplica para el precio de bolsa nacional, el cual retorna el precio promedio ponderado por la generación de dicha variable.

# Manejo de fechas relativas

El formato de fecha preferiblemente debe ser utilizado como YYYY-MM-DD. Otro aspecto relevante para tener en cuenta al momento de desarrollar consultas a _Bix_ es su capacidad para comprender fechas relativas, a continuación presentamos las frases que hacen referencia a periodos de tiempo que el chatbot reconoce:

* Ayer
* Últimos _n_ días
* Semana pasada
* último mes

# Variables disponibles para consultarle a _Bix_



## Rangos de fechas máximos por consulta

# Ejemplos de uso
