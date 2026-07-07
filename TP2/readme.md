# Trabajo Práctico Prolog

Este repositorio contiene la resolución de los ejercicios del TP de Prolog.

---

## Ejercicio 1.1
Clasificar las siguientes secuencias como **átomos**, **variables** o **ninguno**:

| Secuencia                   | Átomo | Variable | Ninguno |
|------------------------------|-------|----------|---------|
| Vincent                      |       | X        |         |
| Masaje de pies               |       |          | X       |
| variable23                   | X     |          |         |
| Variable2000                 |       | X        |         |
| big_kahuna_burger            | X     |          |         |
| 'Gran hamburguesa kahuna'    | X     |          |         |
| Hamburguesa Kahuna Grande    |       |          | X       |
| 'Jules'                      | X     |          |         |
| _Jules                       |       | X        |         |
| '_Jules'                     | X     |          |         |

---

## Ejercicio 1.2
¿Cuáles de las siguientes secuencias de caracteres son átomos, cuáles son 
variables, cuáles son términos complejos y cuáles no son términos en absoluto? Dar el 
funtor y la aridad de cada término complejo.

| # | Secuencia | Átomo | Variable | Término complejo | Ninguno | Funtor | Aridad |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | amores(Vincent,mia) |  |  | **X** |  | amores | 2 |
| 2 | 'amores(Vincent,mia)' | **X** |  |  |  |  |  |
| 3 | Butch(boxeador) |  |  |  | **X** |  |  |
| 4 | boxeador(Butch) |  |  | **X** |  | boxeador | 1 |
| 5 | y(grande(hamburguesa), kahuna(hamburguesa)) |  |  | **X** |  | y | 2 |
| 6 | y(grande(X),kahuna(X)) |  |  | **X** |  | y | 2 |
| 7 | _and(grande(X),kahuna(X)) |  |  | **X** |  | _and | 2 |
| 8 | (Butch mata a Vincent) |  |  |  | **X** |  |  |
| 9 | mata(Butch, Vincent) |  |  | **X** |  | mata | 2 |
| 10 | mata(Butch Vincent) |  |  |  | **X** |  |  |

---

## Ejercicio 1.3
¿Cuántos hechos, reglas, cláusulas y predicados hay en la siguiente base de 
conocimientos? ¿Cuáles son los encabezados de las reglas y cuáles son los objetivos que 
contienen?

---

## 📌 Base de conocimientos dada
```prolog
woman(vincent).
woman(mia).
man(jules).
person(X):- man(X); woman(X).
loves(X,Y):- father(X,Y).
father(Y,Z):- man(Y), son(Z,Y).
father(Y,Z):- man(Y), daughter(Z,Y).
```

---

## 🔎 Análisis

### 1. **Hechos**
Son cláusulas sin condiciones (solo un predicado con argumentos).
- `woman(vincent).`
- `woman(mia).`
- `man(jules).`

👉 **Cantidad de hechos: 3**

---

### 2. **Reglas**
Son cláusulas con `:-` (condiciones).
- `person(X):- man(X); woman(X).`
- `loves(X,Y):- father(X,Y).`
- `father(Y,Z):- man(Y), son(Z,Y).`
- `father(Y,Z):- man(Y), daughter(Z,Y).`

👉 **Cantidad de reglas: 4**

---

### 3. **Cláusulas**
Cada hecho o regla es una cláusula.  
👉 **Total de cláusulas: 7 (3 hechos + 4 reglas)**

---

### 4. **Predicados**
Un predicado se identifica por su nombre y aridad.  
En esta base aparecen:

- `woman/1`  
- `man/1`  
- `person/1`  
- `loves/2`  
- `father/2`  
- `son/2`  
- `daughter/2`

👉 **Cantidad de predicados distintos: 7**

---

### 5. **Encabezados de las reglas y objetivos**
- Regla: `person(X):- man(X); woman(X).`  
  - Encabezado: `person(X)`  
  - Objetivos: `man(X); woman(X)`  

- Regla: `loves(X,Y):- father(X,Y).`  
  - Encabezado: `loves(X,Y)`  
  - Objetivo: `father(X,Y)`  

- Regla: `father(Y,Z):- man(Y), son(Z,Y).`  
  - Encabezado: `father(Y,Z)`  
  - Objetivos: `man(Y), son(Z,Y)`  

- Regla: `father(Y,Z):- man(Y), daughter(Z,Y).`  
  - Encabezado: `father(Y,Z)`  
  - Objetivos: `man(Y), daughter(Z,Y)`  


---
---

## 📌 Ejercicio 1.4 – Represente lo siguiente en Prolog:

1. **Butch es un asesino.**  
```prolog
asesino(butch).
```

2. **Mia y Marsellus están casados.**  
```prolog
casados(mia, marsellus).
casados(marsellus, mia).
```


3. **Zed ha muerto.**  
```prolog
muerto(zed).
```

4. **Marsellus mata a todos los que le dan a Mia un masaje en los pies.**  
```prolog
mata(marsellus, X) :- masaje_pies(X, mia).
```

5. **Mia ama a todos los que son buenos bailarines.**  
```prolog
ama(mia, X) :- buen_bailarin(X).
```

6. **Jules come cualquier cosa que sea nutritiva o sabrosa.**  
```prolog
come(jules, X) :- nutritivo(X).
come(jules, X) :- sabroso(X).
```

---
## Ejercicio 1.5 Supongamos que estamos trabajando con la siguiente base de conocimientos:
```prolog
wizard(ron) .
hasWand(harry) .
quidditchPlayer(harry) .
wizard(X) :- hasBroom(X) , hasWand(X) .
hasBroom(X) :- quidditchPlayer(X) .
```

¿Cómo responde Prolog a las siguientes consultas?

1. Mago(ron)
2. bruja(Ron)
3. Mago(Hermione)
4. Bruja(Hermione)
5. Mago(harry)
6. mago(Y)
7. bruja(Y)


**Respuestas**

1. Mago(Ron). → Error / no válido

2. bruja(ron). → false

3. Mago(Hermione). → Error / no válido

4. Bruja(Hermione). → Error / no válido

5. Mago(Harry). → Error / no válido

6. mago(Y). → false

7. bruja(Y). → false

