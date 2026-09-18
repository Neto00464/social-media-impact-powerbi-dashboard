# 📊 Impacto de las Redes Sociales en la Vida Estudiantil — Power BI Dashboard

Análisis de un dataset de **4,500 estudiantes** (bachillerato a posgrado) para explorar la relación entre el uso de redes sociales, la calidad del sueño, el estrés percibido, la salud mental y el rendimiento académico.

![Vista general del dashboard](screenshots/An%C3%A1lisis%20del%20impacto%20de%20redes%20sociales%20en%20sue%C3%B1o%2C%20estr%C3%A9s%20y%20rendimiento%20acad%C3%A9mico%20Dashboard.PNG)

---

## 🎯 Objetivo del proyecto

Practicar el flujo completo de un análisis de **Business Intelligence**, desde la limpieza y preparación de datos en Python hasta el modelado, análisis y visualización en Power BI.

El proyecto utiliza datos sobre comportamiento digital y bienestar estudiantil para identificar patrones relacionados con el uso de redes sociales, estrés, sueño y rendimiento académico.

---

## ❓ Preguntas de investigación

1. ¿Cómo se relacionan la edad, el uso de redes sociales y el estrés percibido?
2. ¿Cuál es la relación entre el tiempo diario de uso de redes sociales y el GPA?
3. ¿Qué características distinguen a los estudiantes clasificados con impacto `Beneficial` frente a aquellos con impacto `Negative`?
4. ¿Cuáles son las plataformas más utilizadas por los estudiantes?
5. ¿Existe alguna relación entre el uso de redes sociales, la calidad del sueño y la salud mental?

---

## 🗂️ Fuente de datos

* **Dataset:** [Impact of Social Media on Life](https://www.kaggle.com/datasets/harishyadav0506/impact-of-social-media-on-life)
* **Fuente:** Kaggle
* **Autor del dataset:** Harish Yadav
* **Licencia:** CC0 / Dominio público
* **Registros:** 4,500
* **Columnas:** 16

---

## 🛠️ Herramientas utilizadas

| Herramienta          | Uso                                  |
| -------------------- | ------------------------------------ |
| **Python / pandas**  | Limpieza y preparación de datos      |
| **Power BI Desktop** | Modelado, DAX y visualización        |
| **DAX**              | Creación de medidas y KPIs           |
| **Kaggle Notebooks** | Desarrollo del proceso de limpieza   |
| **GitHub**           | Control de versiones y documentación |

---

## 🧹 Proceso de limpieza de datos

Antes de construir el dashboard se realizó un proceso de preparación de los datos utilizando Python y pandas.

Principales transformaciones:

* Unificación de categorías duplicadas por idioma, por ejemplo:

  * `Femenino` → `Female`
  * `Masculino` → `Male`
* Tratamiento de valores nulos.
* Imputación de valores faltantes utilizando la **mediana** de cada variable.
* Estandarización de categorías para facilitar el análisis en Power BI.
* Preparación del dataset para el modelado y visualización.

### Valores imputados

* `Perceived_Stress_Score`: **46 valores**
* `Academic_Performance_GPA`: **85 valores**


---

## 📊 Dashboard

El dashboard contiene diferentes visualizaciones y segmentaciones para explorar los datos desde múltiples perspectivas.

### KPIs principales

* **GPA promedio:** 3.43
* **Estrés promedio:** 13.51
* **Total de estudiantes:** 4,500

### Visualizaciones

* **Top 5 plataformas más utilizadas**
* **Overall Impact vs. Estrés**
* **Overall Impact vs. Salud Mental**
* **Edad vs. Horas de uso**
* **Edad vs. Estrés**
* **Uso diario vs. GPA**
* **Overall Impact vs. Calidad del Sueño**
* **Overall Impact vs. GPA**
* **Matriz resumen de métricas**
* Segmentación por:

  * Nivel académico
  * Género

---

## 📈 Hallazgos principales

### 1. El estrés presenta una diferencia importante entre categorías de impacto

Los estudiantes clasificados como `Negative` presentan un estrés promedio de **31.0**, mientras que el grupo `Beneficial` presenta un promedio de **11.2**.

### 2. El grupo `Negative` presenta mayor tiempo diario de uso

El promedio de uso diario de redes sociales fue:

| Overall Impact | Horas diarias |
| -------------- | ------------: |
| Beneficial     |        4.42 h |
| Negative       |       12.25 h |

### 3. Uso diario y rendimiento académico

El gráfico de dispersión muestra una **tendencia negativa** entre las horas de uso diario y el GPA.

El GPA promedio observado fue:

| Overall Impact |  GPA |
| -------------- | ---: |
| Beneficial     | 3.54 |
| Negative       | 2.56 |

> Estos resultados describen asociaciones observadas dentro del dataset y no deben interpretarse como evidencia de causalidad.

### 4. Salud mental

El índice promedio de salud mental fue:

| Overall Impact | Salud mental |
| -------------- | -----------: |
| Beneficial     |         84.3 |
| Negative       |         47.1 |

### 5. Distribución del impacto

La distribución de estudiantes fue:

* **Beneficial:** 3,681
* **Negative:** 165
* Resto: otras categorías de impacto

Esto muestra que las categorías de impacto no están distribuidas de manera uniforme en el dataset.

### 6. Plataformas más utilizadas

**Instagram** y **TikTok** aparecen entre las plataformas con mayor número de usuarios dentro del dataset, mientras que **Reddit** aparece en el último lugar del Top 5 mostrado en el dashboard.

### 7. Uso adicional durante los fines de semana

`Weekend_Extra_Hours` presenta valores muy similares entre las categorías de impacto, aproximadamente entre **1.73 y 1.80 horas**, por lo que presenta una diferencia menor entre grupos que el uso diario.

---

## 📁 Archivos del proyecto

```text
social-media-impact-powerbi-dashboard/
│
├── Social Media Impact.pbix
├── notebook.ipynb
├── README.md
│
└── screenshots/
    └── Análisis del impacto de redes sociales en sueño, estrés y rendimiento académico Dashboard.PNG
```

### 📊 Power BI

[Descargar / ver archivo PBIX](https://github.com/Neto00464/social-media-impact-powerbi-dashboard/blob/main/Social%20Media%20Impact.pbix)

---

## 📸 Dashboard Preview

![Dashboard](screenshots/An%C3%A1lisis%20del%20impacto%20de%20redes%20sociales%20en%20sue%C3%B1o%2C%20estr%C3%A9s%20y%20rendimiento%20acad%C3%A9mico%20Dashboard.PNG)

---

## 🔗 Power BI Report

El reporte se encuentra publicado en Power BI Service:

[Ver reporte en Power BI](https://app.powerbi.com/groups/me/reports/f03400a4-6d16-4b60-b044-232eb684f2ca/67c777fdd9b59633a35e?experience=power-bi)

> **Nota:** este enlace puede requerir autenticación de Power BI. El reporte público mediante "Publish to web" no está habilitado actualmente para esta cuenta.

---

## 👤 Autor

**José Ernesto Gomez Guido**

* 💼 LinkedIn: [LinkedIn](https://www.linkedin.com/in/ernesto-gomez/)
* 📊 Focus: Data Analytics | Power BI | SQL | Business Intelligence
