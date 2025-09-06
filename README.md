# 🤖 Modelado de Problemas con Espacios de Estados

Este proyecto reúne diferentes ejemplos de **problemas de búsqueda** y **espacios de estados** aplicados a situaciones simples y didácticas.  
La idea central es entender cómo **un agente** (lámpara, mascota, jugador, etc.) puede pasar de un **estado inicial** a un **estado meta** utilizando un conjunto de **acciones disponibles**.

---

## 📘 Teoría Básica

### 🔹 Espacio de Estados
Conjunto de todas las configuraciones posibles de un problema.  
Ejemplo: en una lámpara puede ser `{Encendida, Apagada}`.

### 🔹 Espacio de Acciones
Conjunto de movimientos o transiciones que permiten cambiar de un estado a otro.  
Ejemplo: `{Prender, Apagar}`.

### 🔹 Estado Inicial
Situación de partida desde donde se comienza la búsqueda.

### 🔹 Estado Meta
Condición final o deseada.  
Ejemplo: que la lámpara quede **encendida** o que un jugador llegue al **tesoro**.

### 🔹 Función de Transición
Regla que define cómo un estado cambia a otro dado una acción.

### 🔹 Heurística
En problemas más complejos, se usan funciones que estiman cuán cerca estamos de la meta.  
Ejemplo: en un laberinto, la **distancia Manhattan** es usada para estimar la cercanía al objetivo.

---

## 📊 Resumen de los Ejemplos

| Problema         | Espacio de Estados                        | Acciones                             | Objetivo                               |
|------------------|-------------------------------------------|---------------------------------------|-----------------------------------------|
| **Lámpara**      | Encendida / Apagada                       | Prender, Apagar                       | Encender la lámpara                     |
| **Mascota**      | Feliz / Triste                            | Alimentar (cantidad aleatoria)        | Mantenerla feliz                        |
| **Tesoro**       | Posiciones en una grilla 3x3              | Mover: arriba, abajo, izq, der        | Llegar al tesoro en (2,2)               |
| **Laberinto**    | Posiciones en un tablero con obstáculos   | Mover: arriba, abajo, izq, der        | Llegar a la meta evitando obstáculos    |
| **8-Puzzle**     | Configuraciones del tablero 3x3           | Mover fichas vacías en direcciones    | Reordenar hasta el estado meta          |

---

## 📝 Explicación de los Códigos

### 1. 💡 Lámpara
Un problema simple donde sólo existen dos estados: **encendida** y **apagada**.  
El objetivo es llegar al estado meta (encendida) aplicando la acción adecuada.

---

### 2. 🐶 Mascota
Aquí se introduce la **aleatoriedad**:  
- Si recibe **10 de comida**, queda **feliz**.  
- Si recibe menos, queda **triste**.  
El objetivo es mantener a la mascota en un estado positivo.

---

### 3. 🏴‍☠️ Búsqueda del Tesoro
Un jugador inicia en la posición `(0,0)` y debe llegar al tesoro en `(2,2)`.  
Las acciones disponibles son **moverse en cuatro direcciones**.  
El algoritmo guía los movimientos de forma que siempre se acerque a la meta.

---

### 4. 🧩 Laberinto
Se complica el problema añadiendo **obstáculos**.  
Aquí se usa el **algoritmo A\*** con **heurística Manhattan** para encontrar la ruta más corta evitando colisiones.  
El estado inicial y meta están fijos, pero los obstáculos son aleatorios.

---

### 5. 🔢 8-Puzzle
Un clásico de la inteligencia artificial.  
El tablero tiene fichas que deben moverse para alcanzar una configuración específica.  
El espacio de estados es muy grande, y se requieren **heurísticas** para guiar la búsqueda hacia el objetivo.

---

## 🎯 Finalidad del Proyecto
Estos ejemplos permiten:
- Comprender cómo modelar problemas con **estados, acciones y metas**.  
- Diferenciar entre entornos **deterministas**, **aleatorios** y **con heurísticas**.  
- Dar una introducción práctica a los algoritmos de búsqueda en Inteligencia Artificial.

---

