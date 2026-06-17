# Sistema de Detección de Anomalías en Inventarios de Producción


## 1. Descripción del Proyecto
Este proyecto tiene como objetivo desarrollar un modelo de analítica avanzada en Python para detectar anomalías en los ajustes de inventario de materia prima y semielaborados.
El sistema permitirá identificar automáticamente diferencias atípicas en cantidad y valor, optimizando el proceso de revisión y reduciendo errores humanos.


## 2. Problema de Negocio
Actualmente, el proceso de cierre de inventario se realiza de manera semanal, donde cada área realiza conteos físicos y los compara con el inventario teórico en **SAP**.

Este proceso presenta varios desafíos:
- Alto volumen de datos para revisión manual
- Riesgo de omitir diferencias significativas
- Dependencia del criterio humano
- Posibles impactos financieros por ajustes incorrectos


## 3. Objetivo del Proyecto
Desarrollar un modelo que permita:

- Identificar anomalías en los ajustes de inventario
- Priorizar los casos críticos para revisión
- Reducir el riesgo de errores en el control de inventarios
- Apoyar la toma de decisiones basada en datos

## 4. Datos Utilizados
Se utilizarán las siguientes fuentes de información:

🔹 **Ajustes históricos de inventario**
obtenidos mediante transacción SAP **MI24**

🔹 **Movimientos de inventario**
Se utilizará los movimientos que hubo en la semana de cada materia prima, en relacion a los ingresos y consumos, para ello se utilizará la transaccion **MB51**

## 5. Metodología
El proyecto se desarrollará siguiendo las siguientes etapas:

- Limpieza y preparación de datos

Validación de datos faltantes
Estandarización de variables

-  Análisis exploratorio (EDA)

Distribución de diferencias
Identificación de patrones por área y material
Diferencia absoluta y porcentual
Impacto económico
Z-score por material
Frecuencia de ajustes

- Modelado
Se aplicarán modelos de detección de anomalías como:

Reglas estadísticas (umbrales)
(analizando otros)

- Evaluación

Validación con casos históricos
Comparación con decisiones reales

##6. Tecnologías Utilizadas

Python
Pandas
NumPy
Matplotlib / Seaborn


## 7. Resultados Esperados

- Identificación automática de ajustes anómalos
- Clasificación de riesgos (alto, medio, bajo)
- Reducción del tiempo de revisión manual
- Mejora en la precisión del control de inventarios

## 8. Impacto en el Negocio

- Optimización del proceso de cierre de inventarios
- Disminución de errores humanos
- Mejora en el control financiero
- Mayor trazabilidad y control de materiales

## 9. Autor
Duberney Velez Moreno
Auxiliar de Control de Producción