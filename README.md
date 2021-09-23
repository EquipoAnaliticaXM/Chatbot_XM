
<p align="center"> 
<img src="https://user-images.githubusercontent.com/69567089/132707858-021aeaf4-8cf9-44e9-b4d3-0350b60418de.png">
</p> 


# Índice
1. [Conceptos generales del Chatbot (_Bix_) para consultar variables del Mercado de Energía Mayorista](#section1)
2. [Operaciones aritméticas habilitadas](#section2)
4. [Manejo de fechas relativas](#section3)
5. [Variables disponibles para consultarle a _Bix_ y filtros](#section4)
6. [Ejemplos de uso](#section5)


<p align="center"> 
<img src="https://user-images.githubusercontent.com/69567089/134450647-54c1e086-7069-4b6f-8cb3-8e79018fb882.png">
</p> 

<a id='section1'></a>
# Conceptos generales del Chatbot (_Bix_) para consultar variables del Mercado de Energía Mayorista
Este repositorio se crea con el objetivo de presentar la documentación de uso para la interfaz conversacional creada por el Equipo de Analítica para consultar las principales variables del Mercado de Energía Mayorista y así facilitar el análisis ejecutivo de información específica. El chatbot recibe el nombre de _Bix_ y llega a complementar del abanico de soluciones que tiene disponible XM para mantener actualizados a los diferentes públicos de interés. 

_Bix_ es un chatbot de tipo _basado en reglas_ por lo cual tiene la capacidad de seguir una serie de reglas y comprender palabras claves o frases típicas para responder preguntas sobre la evolución de variables del Mercado de Energía Mayorista. También, mediante el reconocimiento del texto de la conversación, _Bix_ se encuentra en capacidad de realizar operaciones básicas que detallaremos más adelante en esta documentación.

Dentro de las principales funciones en las que _Bix_ puede asistir son:

* Extracción información de una variable del Mercado de Energía Mayorista.
* Exportación de los datos consultados a archivos de Excel.
* Generación de gráficas para facilitar análisis a partir del resultado obtenido.

Las interacciones con el chatbot pueden ser indicadas utilizando lenguaje natural controlado o señalando los comandos que van surgiendo en la pantalla a medida que se desarrolla la conversación.

Es importante resaltar que el idioma oficial de _Bix_ es Español (Colombia).

<a id='section2'></a>
# Operaciones aritméticas habilitadas

 _Bix_ tiene la capacidad de realizar las siguientes operaciones utilizando como fuente la [API XM](https://github.com/EquipoAnaliticaXM/API_XM):

* **Máximo:** Retorna el valor máximo para el periodo de tiempo consultado
* **Mínimo:** Retorna el valor mínimo para el periodo de tiempo consultado
* **Promedio:** Retorna el promedio aritmético para el periodo de tiempo consultado
* **Promedio diario:** Retorna el promedio aritmético diario para el periodo de tiempo consultado
* **Máximo diario:** Retorna el valor máximo observado para cada día dentro del periodo de tiempo consultado
* **Mínimo diario:** Retorna el valor mínimo observado para cada día dentro del periodo de tiempo consultado
* **Promedio ponderado diario:** Aplica para el precio de bolsa nacional, el cual retorna el precio promedio ponderado por la generación real del Sistema Interconectado Nacional.

<a id='section3'></a>
# Manejo de fechas relativas

El formato de fecha a utilizar con _Bix_ debe ser preferiblemente YYYY-MM-DD. Otro aspecto relevante para tener en cuenta al momento de realizar consultas a _Bix_ es su capacidad para comprender fechas relativas, a continuación presentamos las frases que hacen referencia a periodos de tiempo que el chatbot reconoce:

* Ayer
* Últimos _n_ días
* Semana pasada
* Último mes

<a id='section4'></a>
# Variables disponibles para consultarle a _Bix_ y filtros

<details>
<summary>Hidrología</summary>
<ul>
<li>Aporte hídricos en energía</li> 
  <b>Opciones de consulta por:</b> 
    <ul><li>[x] Sistema </li><li>[x] Río</li></ul>
<li>Capacidad Útil energía por embalse</li>
  <b>Opciones de consulta por:</b> 
    <ul><li>[x] Sistema </li><li>[x] Embalse</li></ul>
<li>Media Histórica por Rio</li>
   <b>Opciones de consulta por:</b> 
    <ul><li>[x] Sistema </li><li>[x] Río</li></ul>
<li>Volumen Útil</li>
   <b>Opciones de consulta por:</b> 
    <ul><li>[x] Sistema </li><li>[x] Embalse</li></ul>
</ul>
</details>

<details>
<summary>Demanda</summary>
<ul>
<li>Demanda Comercial</li>
  <b>Opciones de consulta por:</b> 
    <ul><li>[x] Sistema </li><li>[x] Agente</li></ul>
<li>Demanda Comercial No Regulada</li>
  <b>Opciones de consulta por:</b> 
    <ul><li>[x] Sistema </li><li>[x] Agente</li></ul>
<li>Demanda Comercial Regulada</li>
  <b>Opciones de consulta por:</b> 
    <ul><li>[x] Sistema </li><li>[x] Agente</li></ul>
<li>Demanda del SIN</li>
</ul>
</details>

<details>
<summary>Oferta y Generación</summary>
<ul>
<li>Capacidad Efectiva Neta por recurso</li>
<li>Consumo combustible por recurso</li>
<li>Disponibilidad Real por recurso</li>
<li>Generación Fuera de Mérito por recurso</li>
<li>Generación Programada Redespacho por recurso</li>
<li>Generación Real</li>
  <b>Opciones de consulta por:</b> 
    <ul><li>[x] Sistema </li><li>[x] Recurso</li></ul>
</ul>
</details>

<details>
<summary>Transacciones y Precios</summary>
<ul>
<li>DDV Contratada por recurso</li>
<li>Desviaciones al programa de generación por recurso</li>
<li>MC</li>
<li>Obligaciones de Energía Firme por recurso</li>
<li>Precio de Bolsa Nacional</li>
<li>Precio de Escasez de Activación</li>
<li>Precio de Oferta del Despacho</li>
<li>Precio Promedio Contratos No Regulados </li>
<li>Precio Promedio Contratos Regulados</li>
<li>Remuneración Real Individual Diaria del Cargo por Confiabilidad</li>
<li>Restricciones Aliviadas</li>
</ul>
</details>

<details>
<summary>Intercambios Internacionales</summary>
<ul>
<li> Importaciones en Energía </li>
<li> Exportaciones en Energía </li> 
</ul>
</details>

<details>
<summary>Cálculo de emisiones de CO<sub>2</sub></summary>
<ul>
<li> Emisiones de CO<sub>2</sub>eq </li>
</ul>
</details>

<a id='section5'></a>
# Ejemplos de uso

En esta sección se presentan algunos videos tutoriales que ejemplifican cómo se realiza la interacción con _Bix_:



<a id='section6'></a>
# Limitaciones de _Bix_


