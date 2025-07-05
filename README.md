# Análisis de Embudo de Conversión y Test A/A/B – Proyecto Sprint 11

## Descripción del Proyecto

Este proyecto fue desarrollado como parte del Sprint 11 del bootcamp de análisis de datos de TripleTen. El objetivo es analizar el comportamiento de los usuarios dentro de una aplicación de venta de productos alimenticios, estudiar el embudo de conversión y evaluar los resultados de un experimento A/A/B para determinar el impacto de un cambio en el diseño de fuentes.

---

## Etapas del Proyecto

### 1. Preparación de Datos

**Dataset utilizado:** `logs_exp_us.csv`

- Renombrado de columnas para mayor claridad.
- Conversión de tipos de datos (fechas y horas).
- Extracción de columnas adicionales: fecha, hora, día de la semana.
- Validación de integridad y cobertura temporal de los datos.

---

### 2. Análisis General del Comportamiento

- Conteo total de eventos y usuarios únicos.
- Cálculo del promedio de eventos por usuario.
- Identificación del periodo de datos confiables.
- Verificación de la distribución de usuarios entre los grupos experimentales (ExpId 246, 247, 248).

---

### 3. Análisis del Embudo de Conversión

- Identificación y ordenamiento de eventos por frecuencia.
- Cálculo de la proporción de usuarios que completan cada etapa del embudo.
- Análisis de pérdida de usuarios entre etapas.
- Determinación del porcentaje de usuarios que completan todo el embudo hasta el pago.

---

### 4. Análisis del Test A/A/B

- Verificación de la distribución de usuarios por grupo (control A1, control A2, prueba B).
- Comparación de métricas clave entre los grupos:
  - Frecuencia de eventos
  - Conversión por evento
- Pruebas estadísticas (Mann–Whitney U) para evaluar diferencias significativas.
- Evaluación de la validez del experimento y consistencia entre los grupos de control.

---

## Hipótesis Evaluadas

- **H₀:** No hay diferencia significativa entre los grupos de control (ExpId 246 vs. 247).
- **H₁:** Hay diferencia significativa entre los grupos de control.

- **H₀:** No hay diferencia significativa entre el grupo de prueba (248) y los grupos de control combinados.
- **H₁:** Hay diferencia significativa en la conversión o comportamiento de eventos.

**Nivel de significancia:** α = 0.05  
**Corrección por pruebas múltiples:** Aplicación de Bonferroni si es necesario.

---

## Resultados

- Se identificó la etapa del embudo con mayor pérdida de usuarios.
- Los grupos de control mostraron comportamientos consistentes, validando la prueba.
- El grupo de prueba no presentó diferencias estadísticamente significativas en la mayoría de los eventos, lo que sugiere que el cambio de fuente no afectó negativamente la experiencia del usuario.

---

## Tecnologías Utilizadas

- Python  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- SciPy (pruebas estadísticas)  
- Jupyter Notebook

---

## 📫 Contacto

Paz Emmanuel Balderas Cerezo  
📧 pazemmanuel24032005@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/paz-emmanuel-balderas-cerezo-dataanalyst)
