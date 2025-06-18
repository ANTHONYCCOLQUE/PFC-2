# PFC-2
# LangChain con Excel

## Descripción

 **LangChain**, una librería poderosa para construir aplicaciones basadas en agentes de IA. El objetivo de este proyecto es combinar la potencia de LangChain con OpenAI para trabajar con datos estructurados, como los de un archivo Excel. En este caso, se utiliza un conjunto de datos sobre los pasajeros del Titanic para demostrar cómo los agentes pueden interactuar con tablas de datos, proporcionando respuestas a consultas y análisis.

## Propósito

El propósito principal de este proyecto es demostrar cómo utilizar LangChain para integrar agentes con datos tabulares, facilitando la creación de aplicaciones interactivas que pueden procesar grandes cantidades de información de manera eficiente.

## Requisitos
Para poder ejecutar este proyecto, necesitas instalar las siguientes librerías de Python. Esto se puede hacer fácilmente utilizando pip:
- **langchain**: Framework que facilita la integración de modelos de lenguaje con herramientas externas.
- **langchain_openai**: Permite integrar OpenAI GPT con LangChain.
- **langchain_experimental**: Proporciona herramientas experimentales para nuevos tipos de agentes.
- **pandas**: Librería para manipulación y análisis de datos.
- **numpy**: Librería para operaciones matemáticas.
- **tabulate**: Herramienta para mostrar tablas de manera legible.
- **openpyxl**: Para leer y escribir archivos Excel.
  
``pip install langchain langchain_openai langchain_experimental pandas numpy tabulate openpyxl -q``

## Uso
El código principal se encuentra en el archivo LanghChain_con_Excel.ipynb. A continuación, se proporciona un ejemplo básico de cómo usar el proyecto.

### Codigo de ejemplo
Importa las librerías necesarias:

![](https://github.com/ANTHONYCCOLQUE/t44/blob/main/librerias.png)


Carga el archivo Excel con los datos del Titanic:

``df = pd.read_excel("titanic.xlsx")
  df.head()``
  
![](https://github.com/ANTHONYCCOLQUE/t44/blob/main/df.png)



Crea un agente que interactúe con el dataframe:

![](https://github.com/ANTHONYCCOLQUE/t44/blob/main/agente.png)


Realiza una consulta al agente para obtener información sobre los datos:

![](https://github.com/ANTHONYCCOLQUE/t44/blob/main/result.png)

Este código cargará los datos del Titanic desde un archivo Excel y creará un agente que puede hacer preguntas sobre esos datos.
###Ejemplos de preguntas que el agente puede responder:
- ¿Cuántos pasajeros sobrevivieron en el Titanic?
- ¿Cuál es la edad promedio de los pasajeros?
- ¿Cuántos pasajeros pagaron más de una cierta tarifa?
- ¿Cuántos hombres y cuántas mujeres había a bordo?
