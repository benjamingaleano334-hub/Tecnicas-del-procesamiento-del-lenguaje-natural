
# Consigna 1 – Modelo de Claves Booleanas

Este proyecto implementa un sistema de **búsqueda booleana (AND, OR, NOT)** sobre un conjunto de documentos relacionados con **Inteligencia Artificial y Aprendizaje Automático**, utilizando **NLTK** en Python.

---

## 📂 Contenido
- `busqueda_booleana1.ipynb`: notebook con la implementación paso a paso.
- `README.md`: este archivo con instrucciones y ejemplos.

---

## 🚀 Ejecución
1. Abrir Jupyter Notebook.
2. Cargar `BooleanSearch_Consigna1.ipynb`.
3. Ejecutar todas las celdas.
4. Ingresar consultas booleanas en la terminal/notebook.  
   Para salir, escribir `salir`.

---

## 📖 Documentos utilizados
```text
"doc1": "La inteligencia artificial está revolucionando la tecnología."
"doc2": "El aprendizaje automático es clave en la inteligencia artificial."
"doc3": "Procesamiento del lenguaje natural y redes neuronales."
"doc4": "Las redes neuronales son fundamentales en deep learning."
"doc5": "El futuro de la IA está en el aprendizaje profundo."
```

---

## 🔎 Ejemplos de consultas
```text
Ingrese una consulta booleana (o 'salir' para terminar): inteligencia AND artificial
📄 Documentos encontrados: {'doc1', 'doc2'}

Ingrese una consulta booleana (o 'salir' para terminar): redes OR aprendizaje
📄 Documentos encontrados: {'doc2', 'doc3', 'doc4', 'doc5'}

Ingrese una consulta booleana (o 'salir' para terminar): inteligencia NOT automatico
📄 Documentos encontrados: {'doc1'}
```

---

## ✅ Notas
- Los operadores booleanos (`AND`, `OR`, `NOT`) pueden escribirse en mayúsculas, minúsculas o mezclados (`and`, `And`, `AND`).
- Las palabras con acento también se reconocen aunque se escriban sin acento (`automatico` = `automático`).
- El sistema utiliza un **índice invertido** para asociar cada palabra con los documentos en los que aparece.

---

## 🛠️ Tecnologías utilizadas
- Python 3
- NLTK (tokenización)
- Jupyter Notebook

