# 📊 Impacto de las Redes Sociales en la Vida Estudiantil — Dashboard en Power BI

Análisis de un dataset de 4,500 estudiantes (bachillerato a posgrado) explorando cómo el uso de redes sociales se relaciona con la calidad del sueño, el estrés percibido, la salud mental y el rendimiento académico.

![Vista general del dashboard](screenshots/overview.png)

## 🎯 Objetivo del proyecto

Practicar el flujo completo de un análisis de Business Intelligence: desde la limpieza de datos en Python hasta la construcción de un dashboard interactivo en Power BI, aplicado a un caso real de comportamiento digital y bienestar estudiantil.

## ❓ Preguntas de investigación

1. ¿Cómo influye el uso nocturno de pantallas y la edad en los patrones de uso y estrés?
2. ¿Cuál es la relación empírica entre el tiempo diario de pantalla y el promedio académico (GPA)?
3. ¿Qué distingue a los estudiantes clasificados con impacto "Beneficial" de aquellos con impacto "Negative"?
4. ¿Cuáles son las plataformas más usadas entre los estudiantes?

## 🗂️ Fuente de datos

* **Dataset:** [Impact of Social Media on Life](https://www.kaggle.com/datasets/harishyadav0506/impact-of-social-media-on-life) — Kaggle, por Harish Yadav
* **Licencia:** CC0 (Dominio público)
* **Tamaño:** 4,500 registros, 16 columnas

## 🛠️ Herramientas utilizadas

* **Python (pandas)** en Kaggle Notebooks — limpieza de datos: unificación de categorías bilingües (español/inglés), manejo de valores nulos (imputación por mediana en `Perceived_Stress_Score` y `Academic_Performance_GPA`)
* **Power BI Desktop** — modelado de datos, medidas DAX y construcción del dashboard interactivo

## 🧹 Proceso de limpieza de datos

* Se unificaron categorías duplicadas por idioma (ej. "Femenino"/"Female" → "Female")
* Se imputaron 46 valores nulos en `Perceived_Stress_Score` y 85 en `Academic_Performance_GPA` usando la mediana de cada columna
* Notebook de limpieza disponible en [`notebook.ipynb`](notebook.ipynb)

## 📊 Contenido del dashboard

* **KPIs generales:** GPA promedio (3.43), Estrés promedio (13.51), Total de estudiantes (4,500)
* **Segmentaciones interactivas:** por Nivel Académico (High School, Undergraduate, Postgraduate) y Género
* **Top 5 Plataformas Más Usadas:** ranking de estudiantes por red social
* **Overall Impact vs Estrés y Salud Mental:** comparación de las 3 categorías de impacto
* **Edad vs Horas de Uso y Estrés:** evolución de estas métricas a través de las edades (15-26 años)
* **Uso Diario vs GPA:** dispersión con línea de tendencia
* **Overall Impact vs Calidad de Sueño y GPA:** comparación de bienestar por categoría
* **Tabla resumen (Matrix):** todas las métricas clave cruzadas por categoría de Overall Impact

## 📈 Hallazgos principales

* **El estrés es el diferenciador más claro entre categorías:** los estudiantes con `Overall_Impact = Negative` reportan un estrés promedio de 31.0, más del doble que los clasificados como `Beneficial` (11.2).
* **El uso diario está fuertemente ligado al impacto:** el grupo `Negative` usa redes sociales 12.25 horas al día en promedio, casi 3 veces más que el grupo `Beneficial` (4.42 horas).
* **Existe una correlación negativa entre uso diario y GPA:** la línea de tendencia del gráfico de dispersión confirma que a más horas de pantalla, el rendimiento académico tiende a bajar (GPA promedio: 3.54 en Beneficial vs 2.56 en Negative).
* **La salud mental sigue el mismo patrón:** índice de salud mental promedio de 84.3 en Beneficial frente a solo 47.1 en Negative.
* **La distribución no es pareja:** la mayoría de los estudiantes (3,681 de 4,500) caen en la categoría Beneficial, mientras que solo 165 están en Negative — sugiere que el uso problemático es la minoría, no la norma, en este dataset.
* **Instagram y TikTok dominan** como las plataformas más usadas por los estudiantes, muy por delante de Reddit, que aparece en último lugar del Top 5.
* **Weekend_Extra_Hours no diferencia bien entre categorías** (1.73–1.80 horas en las tres), lo que sugiere que el tiempo extra de fin de semana no es un factor determinante del impacto general, a diferencia del uso diario entre semana.

## 📊 Ver el dashboard interactivo

🔗 [Ver reporte en vivo](TU_ENLACE_DE_PUBLISH_TO_WEB_AQUI)

## 📁 Contenido del repositorio

```text
├── dashboard.pbix          # Archivo de Power BI
├── notebook.ipynb          # Limpieza de datos en Python (Kaggle)
├── README.md
└── screenshots/            # Capturas de las páginas del dashboard
```

## 👤 Autor

**Tu nombre**

* LinkedIn: (tu enlace)
* Portafolio: (tu enlace)
