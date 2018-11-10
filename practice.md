---
title: "Test"
author: "Joshua Kock"
date: "11/10/2018"
output: 
  html_document: 
    keep_md: yes
---



## Introducción:
Para el presente ejercicio utilizaremos datos de mamografia y cancer de seno disponibles libremente en https://www.kaggle.com/overratedgman/mammographic-mass-data-set, bajo la licencia de CC BY-NC-SA 4.0. Las pacientes fueron reclutados en el año 2007 midiendo variables relacionadas con la mamografia y posteriormente fueron sometidas a biopsia para definir la malignidad o no de los hallzagos imagenologico. Con los presentes datos realizaremos un modelo lineal generalizado logistico. La metodologia a implementar es:

(1) La exploracion inicial de la base de datos y las variables.
(2) La generacion de un Modelo lineal generalizado.
(3) La simplificacion del model (si aplica).
(4) El diagnostico del modelo.
(5) Ajuste del modelo (si es necesario)
(6) Conclusion.

En nuestro ejercicio vamos a establecer a _priori_ como mi variable respuesta la presencia o no de malignidad en la biopsia de seno.

Posteriormente, cargamos los datos del archivo llamado **cancer_seno** y le asignamos el nombre **ca_mama** a los datos; de esta forma se genera un objeto con el nombre gases. Dentro de R este objeto tendrá la característica de ser un dataframe.

```r
ca_mama <-read.csv("cancer_seno.csv", header = TRUE)
```
