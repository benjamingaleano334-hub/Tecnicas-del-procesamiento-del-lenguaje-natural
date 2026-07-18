
# Consigna 2 – Modelo de Claves Booleanas

Este proyecto implementa un sistema de **búsqueda booleana (AND, OR, NOT)** sobre un conjunto de documentos relacionados con **civilizaciones antiguas**, utilizando **NLTK** en Python.

---

## 📂 Contenido
- `busqueda_booleana2.ipynb`: notebook con la implementación paso a paso.
- `README.md`: este archivo con instrucciones y ejemplos.

---

## 🚀 Ejecución
1. Abrir Jupyter Notebook.
2. Cargar `BooleanSearch_Consigna2.ipynb`.
3. Ejecutar todas las celdas.
4. Ingresar consultas booleanas en la terminal/notebook.  
   Para salir, escribir `salir`.

---

## 📖 Documentos utilizados
```text
"doc1": "Los egipcios construyeron las pirámides y desarrollaron una escritura jeroglífica."
"doc2": "La civilización romana fue una de las más influyentes en la historia occidental."
"doc3": "Los mayas eran expertos astrónomos y tenían un avanzado sistema de escritura."
"doc4": "La antigua Grecia sentó las bases de la democracia y la filosofía moderna."
"doc5": "Los sumerios inventaron la escritura cuneiforme y fundaron las primeras ciudades."
```

---

## 🔎 Ejemplos de consultas
```text
Ingrese una consulta booleana (o 'salir' para terminar): egipcios AND pirámides
📄 Documentos encontrados: {'doc1'}

Ingrese una consulta booleana (o 'salir' para terminar): escritura OR astrónomos
📄 Documentos encontrados: {'doc1', 'doc3', 'doc5'}

Ingrese una consulta booleana (o 'salir' para terminar): romano NOT griegos
📄 Documentos encontrados: {'doc2'}
```

---

## ✅ Notas
- Los operadores booleanos (`AND`, `OR`, `NOT`) pueden escribirse en mayúsculas, minúsculas o mezclados (`and`, `And`, `AND`).
- Las palabras con acento también se reconocen aunque se escriban sin acento (`piramides` = `pirámides`).
- El sistema utiliza un **índice invertido** para asociar cada palabra con los documentos en los que aparece.

---

## 🛠️ Tecnologías utilizadas
- Python 3
- NLTK (tokenización)
- Jupyter Notebook

