# Diferenciación del microbioma intestinal entre individuos sanos y pacientes con sepsis mediante secuenciación 16S rRNA

Este repositorio contiene el desarrollo de un proyecto de investigación clínica y bioinformática orientado a comparar la composición del microbioma intestinal entre individuos sanos y pacientes con sepsis. Utiliza técnicas de secuenciación del gen 16S rRNA y análisis computacional mediante la plataforma QIIME2.


## Propósito del proyecto

Explorar cómo varía el microbioma intestinal en el contexto de la sepsis, una condición crítica frecuente en unidades de cuidados intensivos (UCI), con el fin de:

- Detectar alteraciones en la diversidad bacteriana.
- Identificar posibles biomarcadores microbianos asociados al estado séptico.
- Evaluar el potencial diagnóstico del perfil microbiano intestinal.

## Objetivos

### Objetivo general

Diseñar y llevar acabo un estudio clínico-bioinformático para comparar el microbioma intestinal de pacientes sépticos y personas sanas mediante secuenciación 16S y herramientas de análisis computacional.

### Objetivos específicos

- Recolectar y procesar muestras fecales de ambos grupos.
- Realizar extracción de ADN y secuenciación de regiones V3-V4 del gen 16S rRNA.
- Comparar métricas de diversidad alfa y beta entre los grupos.
- Identificar taxones diferenciales relacionados con la sepsis.
- Evaluar el uso del perfil bacteriano como posible biomarcador diagnóstico y pronóstico. 


## Metodología

### Población y muestras

- **Grupo 1**: 30 pacientes adultos con sepsis (muestras tomadas en UCI).
- **Grupo 2**: 30 adultos sanos sin enfermedades previas ni uso reciente de antibióticos.

Las muestras fecales se almacenarán a -80°C y se procesarán con kits comerciales (QIAamp DNA Stool Mini Kit).

### Secuenciación

- Regiones V3-V4 amplificadas por PCR.
- Plataforma: Illumina MiSeq (paired-end, 2x250 pb).
- Barcoding individual por muestra.

### Análisis bioinformático

El procesamiento de datos se realizará con QIIME2. Las etapas incluyen:

- Limpieza y desreplicación con DADA2.
- Asignación taxonómica con la base SILVA 138.
- Análisis de diversidad alfa (Shannon, Faith's PD) y beta (Bray-Curtis, UniFrac).
- Pruebas estadísticas: ANCOM, PERMANOVA.

## Estructura del repositorio

Database: datos.
Scripts: código en R y comandos QIIME2.
Resultados: visualizaciones, estadísticas.
Docs: informe.
