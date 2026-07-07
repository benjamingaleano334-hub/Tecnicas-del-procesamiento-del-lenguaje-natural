# 📊 NLP Pipeline: Análisis de Corpus y Frecuencia de Palabras

Este proyecto implementa un **pipeline de procesamiento de texto (NLP)** aplicado a un corpus sobre lenguajes de programación.  
El objetivo es **canalizar el texto hacia métricas cuantitativas y visualizaciones**, destacando conceptos clave como frecuencia de palabras y TF‑IDF.

---

## 🚀 Objetivos
- Analizar un corpus de frases relacionadas con lenguajes de programación.
- Obtener métricas de frecuencia absoluta y relativa.
- Detectar redundancias dentro de las oraciones.
- Visualizar la distribución de palabras en gráficos claros y ordenados.
- Documentar el flujo como un pipeline reproducible.

---

## 🛠️ Tecnologías utilizadas
- **Python**: procesamiento y análisis de texto.
- **scikit-learn**: `TfidfVectorizer` para calcular relevancia de términos.
- **collections.Counter**: conteo de frecuencia de palabras.
- **matplotlib**: visualización gráfica de distribuciones.
- **Markdown/Jupyter Notebook**: documentación y explicación paso a paso.

---

## 📂 Contenido
- `corpus_limpio`: conjunto de frases sobre lenguajes de programación.
- Código para:
  - Top 6 palabras más usadas.
  - Palabra menos utilizada.
  - Palabras repetidas en la misma oración.
  - Gráfico de distribución de frecuencia (ordenado).
- Informe final con conclusiones.

---

## 📈 Resultados
- **Palabras dominantes**: Python y JavaScript (7 apariciones cada una).
- **Palabras menos frecuentes**: beginner, ecosystem, nature, slower (1 aparición).
- **Repeticiones internas**: términos como *require* y *compilation* aparecen varias veces en la misma oración.
- **Distribución gráfica**: muestra claramente el contraste entre palabras muy frecuentes y términos marginales.

---

## ✅ Conclusiones
El pipeline evidencia:
- Un enfoque comparativo entre lenguajes interpretados y compilados.
- La relevancia de Python y JavaScript en el corpus.
- La importancia de conceptos técnicos como *interpreted*, *compiled*, *require* y *compilation*.
- Un vocabulario balanceado: núcleo de palabras frecuentes + diversidad de términos menos usados.

---

## 🧩 Aprendizajes
Este proyecto combina:
- **Conceptos de NLP** (TF‑IDF, frecuencia de palabras).
- **Visualización de datos** para comunicar resultados.
- **Documentación clara** en Markdown para portafolio profesional.
