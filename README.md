
# Telecom X Challenge — Predicción de Cancelación de Clientes

## Descripción
Este proyecto analiza los factores que influyen en la **cancelación de clientes (evasión)** en Telecom X y compara dos modelos de clasificación supervisada:

- **Regresión Logística**
- **Random Forest**

El objetivo es identificar patrones de cancelación, evaluar el desempeño predictivo de los modelos y proponer estrategias de retención basadas en evidencia.

---

## Objetivos
- Preparar y transformar los datos para modelado.
- Identificar variables relevantes asociadas a la evasión.
- Entrenar y comparar modelos de clasificación.
- Interpretar los resultados desde una perspectiva de negocio.
- Proponer acciones concretas de retención de clientes.

---

## Estructura del notebook
El notebook está organizado en las siguientes etapas:

1. **Carga de datos**
2. **Limpieza y selección de variables**
3. **Codificación de variables categóricas**
4. **Verificación del desbalance de clases**
5. **Escalado de variables numéricas**
6. **Análisis de correlación**
7. **Visualización de variables clave**
8. **Separación de entrenamiento y prueba**
9. **Entrenamiento de modelos**
10. **Evaluación de desempeño**
11. **Análisis de factores más influyentes**
12. **Conclusiones y recomendaciones**

---

## Resultados principales
De acuerdo con los resultados obtenidos:

- **Random Forest** logró mejor desempeño global en términos de **accuracy**.
- **Regresión Logística** mostró mejor capacidad para detectar clientes que cancelan, con mejor **recall** en la clase positiva.
- Las variables más relacionadas con la evasión se concentraron en factores como:
  - tipo de contrato,
  - antigüedad del cliente,
  - cargos mensuales o totales,
  - método de pago,
  - y servicios asociados.

---

## Hallazgos de negocio
Los clientes con mayor probabilidad de cancelación suelen compartir algunas características:
- menor tiempo de permanencia,
- contratos mensuales,
- cargos relativamente altos,
- menor vinculación o integración con otros servicios.

Esto sugiere que la empresa puede mejorar la retención mediante:
- campañas de fidelización temprana,
- incentivos para contratos de mayor duración,
- beneficios personalizados para clientes en riesgo,
- revisión de precios y valor percibido del servicio.

---

## Cómo ejecutar
1. Abrir el notebook en Google Colab o Jupyter.
2. Ajustar la ruta del archivo en la variable:

```python
DATA_PATH = '/content/datos_TelecomX_part1.csv'
```

3. Ejecutar las celdas en orden.


---

## Recomendaciones para la presentación
Durante la exposición conviene resaltar:

1. **Problema de negocio:** predecir qué clientes tienen riesgo de cancelar.
2. **Preparación de datos:** limpieza, encoding y tratamiento del desbalance.
3. **Comparación de modelos:** accuracy, recall, precisión y F1-score.
4. **Factores clave:** variables que más influyen en la cancelación.
5. **Acciones de negocio:** estrategias de retención basadas en resultados.
