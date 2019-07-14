## Introducción a la programación en R

### Objetivo

Este curso pretende ser una introducción al lenguaje R; actualmente R es el principal programa utilizado en el área de estadística y está muy bien posicionado en diferentes disciplinas asociadas a la ciencia de datos, el ánalisis y la visualización. El curso tendrá una gran énfasis práctico y brindará herramientas para que cada estudiante sea capaz de enfrentarse a un conjunto de datos reales logrando procesar dichos datos, analizarlos y presentar los resultados.


### Descripción

**Módulo 1**

- Ejemplos de usos de R en diferentes áreas.
- Características de R. Terminal de R y RStudio.
- Sintaxis de R (.R). Trabajo en proyecto (.Rproj).
- Paquetes y funciones. Usos de las ayudas y foros.

**Módulo 2**

- Objetos: vectores, matrices, marco de datos y listas.
- Operadores: aritméticos, relacionales, lógicos, especiales.
- Estructuras repetitivas y condicionales.
- Manipulación de objetos
- Importación y exportación de archivos.

**Módulo 3**

- Análisis estadístico.
- Visualización de datos (gráficos y mapas).
- Informes reproducibles (.Rmd).

### Presentaciones

---
title: "Introducción a la programación en R<br><br>
![](img/Rlogo.png){ width=8% } &nbsp; ![](img/RStudio-Logo-Flat.png){ width=18% }"
author: "Gabriela Mathieu<br>
<span style = 'font-size: 80%;'>
Escuela de invierno <br>
Taller 15 de julio de 2019<br><br>
</span>"
date: '
![](img/cc-by-sa.png)'

output: 
  xaringan::moon_reader:
    css: [default, default-fonts, custom.css]
    nature:
      highlightStyle: github
      highlightLines: true
---
# Vectores

- Los vectores son la estructura más básica que tenemos para manejar datos en R. 
<br>

- Un escalar también es un vector para R. 
<br>

- Es un tipo de objeto de R. Pero otros objetos están compuestos por vectores: las columnas o filas de una matriz, las variables en un data.frame o una lista, etc. 
<br>

- Comprender cómo se trabaja con un vector en R es fundamental para entender la lógica de R.
<br>

- En este apartado veremos cómo los vectores trabajan con operadores y funciones, y qué significa la 'vectorización'.

---
# Vectores

- Un vector es una colección de uno o más objetos del mismo tipo (números o caracteres pero no ambos).

```{r}
digit <- 1:9
digit
```
--

- A diferencia de otros lenguajes los vectores no son fila o columna, sino una secuencia de valores.
```{r}
dim(digit)
```
--

- Pero si tienen largo que da cuenta de la cantidad de elementos.
```{r}
length(digit)
```

