# Memoria de Proyecto: World Happiness Report

Proyecto de análisis de los indicadores utilizados en la publicación del Work Happiness Report: auditamos calidad del dato, resultados y su metodología a través de sus documentos oficiales.

## Índice

-  [Preambulo: El contexto de los datos](#preambulo-el-contexto-de-los-datos)

- [1. Campos y categorías](#1-campos-y-categorías)

- [2. Patrones generales](#2-patrones)

- [3. Análisis Exploratorio de Datos (EDA)](#3-análisis-exploratorio-de-datos-eda)

- [4. Cambios ejecutados](#4-cambios-ejecutados)

- [5. Nuestras cuestiones sobre los datos](#5-nuestras-cuestiones-sobre-los-datos)

- [7. Visualización como respuesta](#7-visualización-como-respuesta:)

- [8. Next Steps: vistas a futuro](#8-next-steps-pasos-a-futuro)

---
---

## Preambulo: el contexto de los datos

       .

## 1. Campos y categorías

Los ``[datos proporcionados](relative path del o de los archivos)`` para el proyecto de análisis presenta índices como columnas:

- [Nombre del país](#country-name)

- [Indicador regional a nivel global](#regional-indicator)

- [Año](#year)

- [Satisfacción vital](#life-ladder)

- [PIB per cápita en logaritmo natural](#log-gdp-per-capita)


---

## 2. Patrones

|  Generales  |
| ----------- |
| Datos de naturaleza... ``<insertar descripción>``
| ``<insertar el homólogo en este batch de datos>`` a  ``Escalas de valoración (ambiente laboral, satisfacción con el trabajo) sin estandarizar (0-5, 0-50).``
|Columnas duplicadas (``<las que sean``>).
|Columnas que contienen ``<X cosa>``.
|``<más propiedades, como valores boleanos>``.|

---
---
ㅤ     

|  Valores nulos  |
| ----------------|
|``Descripción y distribución``|
---
---
ㅤ     


|  Valores Objeto |
| ----------------|
|``Descripción y distribución``|
---
---
ㅤ     

| Valores Numéricos |
| ------------------|
|``Descripción y distribución``|
---

---
---

ㅤ     

## 3. Análisis Exploratorio de Datos (EDA)


### Country Name

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Regional Indicator

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Year

*Año de la recolección de los datos*


**Propuesta de mejora:**

       > 
ㅤ
**Propuesta ejecutada:**

- 

---
---

### Life Ladder

*Escala de satisfacción vital.*

Las evaluaciones de vida de la encuesta Gallup World Poll son la base para el ranking anual de felicidad. La *escala de Cantril* pide a los encuestados que imaginen una escalera, donde el peldaño 10 representa la mejor vida posible para ellos y el 0, la peor. Luego, se les pide que califiquen su vida actual en una escala del 0 al 10.

**Propuesta de mejora:**

       > 

**Propuesta ejecutada:**

- 

---
---

### Log GDP Per Capita

*Logaritmo del PIB per cápita, que no es lo mismo que PIB per cápita*:

Esta métrica se refiere al logaritmo (generalmente en base 10 o natural) del Producto Interno Bruto (PIB) por persona, ajustado a paridad de poder adquisitivo (PPA) en muchos contextos.

Se utiliza para suavizar la distribución de los datos y **facilitar comparaciones entre países con diferencias económicas muy marcadas**, ya que el logaritmo reduce el impacto de valores extremos y permite analizar el crecimiento relativo en lugar del absoluto.

No trabajamos con el crecimiento absoluto. Podría ser interesante cruzar el dato.



**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Social Support

*Apoyo social percibido*

Usa la media nacional de las respuestas binarias (0=no, 1=sí) a la pregunta de la encuesta Gallup World Poll (GWP): 

>      “Si tuviera problemas, ¿tiene familiares o amigos en quienes pueda confiar para que le ayuden siempre que los necesite, o no?”.

ㅤ
**Propuesta de mejora:**

       > 

**Propuesta ejecutada:**

- 

---
---

### Healthy Life Expectancy At Birth

*Esperanza de vida al nacer.*

 La serie temporal se construye a partir de datos del repositorio de la Organización Mundial de la Salud (OMS). Para cubrir el período de este informe (2005-2022), se utilizan técnicas de interpolación y extrapolación.
ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Freedom To Make Life Choices educationfield

Se usa la media nacional de las respuestas binarias (0-1) a la pregunta de la GWP:

>      “¿Está satisfecho o insatisfecho con su libertad para elegir qué hacer con su vida?”


**Propuesta de mejora:**

       > 

**Propuestas ejecutadas:**

-

---
---

### Generosity

*Cantidad de donaciones en relación con el log. del PIB per cápita*

Se calcula como el residuo de la regresión de la media nacional de las respuestas de la GWP a la pregunta:

>      “¿Ha donado dinero a una organización benéfica en el último mes?” sobre el logaritmo del PIB per cápita.

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Perceptions Of Corruption

Se usa la media de las respuestas binarias (0-1) a dos preguntas de la GWP: 

>      “¿La corrupción está muy extendida en el gobierno o no?”

>       “¿La corrupción está muy extendida en las empresas o no?”

Cuando faltan datos sobre corrupción gubernamental, se utiliza la percepción de corrupción en las empresas como medida general.

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Positive Affect

*Sentimientos positivos experimentados recientemente*

Se define como la media de las medidas de efectos del día anterior para risa, disfrute e interés. La inclusión del interés (**incorporado por primera vez en el Informe Mundial de la Felicidad 2022**) aporta tres componentes tanto al afecto positivo como al negativo, mejorando ligeramente el ajuste del modelo en la columna 4. 

La forma general de las preguntas sobre afecto es: 

>      “¿Experimentó los siguientes sentimientos durante gran parte del día de ayer?”.

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Negative Affect

*Sentimientos negativos experimentados recientemente*

Se define como la media de las medidas de efectos del día anterior para preocupación, tristeza y enojo.

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Confidence In National Government

*Confianza en el Gobierno de la Nación*

Esta variable se calcula a partir de la siguiente pregunta de la encuesta Gallup World Poll:

>      “¿Tiene confianza en el gobierno nacional?”.

Las opciones de respuesta son:
- “Sí, siempre”

- “Sí, a veces”

- “No, rara vez”

- “No, nunca”

- “No sabe”

La variable se calcula como el porcentaje de encuestados que responden ``“Sí, siempre”`` o ``“Sí, a veces”`` a esta pregunta.


ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

## 4. Cambios ejecutados

Propuestas ejecutadas generales y particulares a columnas concretas:

| [Transformaciones](/notebooks/transformación.ipynb)

| [Resultados, datos limpios](``<ruta relativa del archivo de datos limpios>``)

---

## 5. Nuestras cuestiones sobre los datos

Primeras preguntas para enfocar el análisis del proyecto:


---
---

### 6. Pasos previos a la visualización de datos


---
---

#### Resumen de valores atípicos (outliers)

---

---
## 7. Visualización como respuesta


 
---
---


## 8. Next steps: pasos a futuro

``<cuerpo de nuestra teoría que fundamente lo que proyectamos y proponemos con estos datos>``

Por todo esto, concluimos que **la precisión técnica es un imperativo ético**.

### Nuestra propuesta de valor es <blablabla>



### Ampliación del marco ético:

       > ?


### Normalización y Documentación

- Glosario de Valores: Sería necesario un glosario que defina explícitamente el significado de cada valor en las escalas utilizadas.

- Convención de Escala: Documentar formalmente el uso de los valores en las escalas, aunque no aparezcan en los registros actuales.

### Futuras visualizaciones

