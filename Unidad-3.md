[⬅️ Volver al Portafolio](Portafolio-Matematicas-Discretas.md)

---

<h1 align="center">🕸️ UNIDAD 3 · Teoría de Grafos y Árboles</h1>
<p align="center"><i>Modelando conexiones: de las redes sociales a las rutas de un GPS</i></p>

---

## 🧭 Contenido de esta página

| Sección | Tema |
|---|---|
| 🕸️ Parte 1 | Fundamentos de grafos |
| 🌲 Parte 2 | Fundamentos de árboles |
| 🚀 APE | Aprendizaje Práctico Experimental |
| 📖 AA | Aprendizaje Autónomo |
| 👨‍🏫 ACD | Sesiones con el docente |
| 📝 Evaluación | Evaluación integradora |

> 📎 **Nota:** pega el enlace de Google Drive correspondiente en cada marcador `[PEGA_AQUÍ_TU_LINK]`.

---

## 🌍 ¿Por qué importan los grafos y los árboles?

Casi cualquier sistema que "conecta cosas" —personas, ciudades, páginas web, archivos— puede modelarse como una estructura de nodos y enlaces. Esa es exactamente la idea detrás de un grafo, y su versión jerárquica y sin ciclos: el árbol.

| Sistema cotidiano | Estructura detrás |
|---|---|
| Google Maps calculando una ruta | Grafo ponderado + algoritmo de Dijkstra / A* |
| El feed de amistades en redes sociales | Grafo no dirigido (o dirigido, según la red) |
| El explorador de archivos de tu computador | Árbol jerárquico |
| La resolución de nombres de dominio (DNS) | Árbol distribuido |
| Rutas de reparto de un servicio de entregas | Grafo ponderado con optimización de caminos |

---

## 🕸️ Parte 1 — Fundamentos de grafos

### ¿Qué es un grafo?

Un **grafo** es un par de conjuntos: **vértices** (los elementos que se quieren representar) y **aristas** (las relaciones o conexiones entre esos elementos). Es la estructura matemática más flexible para modelar relaciones que no siguen una jerarquía fija.

### Clasificación según su naturaleza

| Tipo de grafo | ¿Qué lo distingue? | Ejemplo real |
|---|---|---|
| No dirigido | Las conexiones no tienen sentido definido | Amistades en Facebook |
| Dirigido | Cada arista tiene un origen y un destino | "Seguir" en Twitter/X |
| Ponderado | Cada arista tiene un costo o peso asociado | Distancias en Google Maps |
| Completo | Todo vértice está conectado con todos los demás | Redes muy pequeñas y densas |
| Bipartito | Los vértices se dividen en dos grupos, sin conexiones internas al mismo grupo | Asignación de tareas a trabajadores |

### ¿Dónde se aplican?

Redes sociales · redes eléctricas · telecomunicaciones · inteligencia artificial · sistemas GPS · videojuegos · redes neuronales · transporte público.

---

## 🌲 Parte 2 — Fundamentos de árboles

### ¿Qué es un árbol?

Un **árbol** es un caso particular de grafo: no dirigido, conexo y **sin ciclos**. Esta simplicidad estructural es justo lo que lo hace tan útil para organizar información de forma jerárquica y acelerar búsquedas.

> 📌 **Propiedad clave:** todo árbol con **n vértices** tiene exactamente **n − 1 aristas**. Ni una más, ni una menos — si tuviera más, existiría un ciclo; si tuviera menos, no estaría conectado.

### Formas de recorrer un árbol

| Recorrido | Orden de visita |
|---|---|
| Preorden | Raíz → Izquierda → Derecha |
| Inorden | Izquierda → Raíz → Derecha |
| Postorden | Izquierda → Derecha → Raíz |

### ¿Dónde se aplican?

Árboles genealógicos · sistemas de archivos · compiladores (árboles de sintaxis) · inteligencia artificial (árboles de decisión) · bases de datos (árboles B) · DNS de Internet · estructuras especializadas como árboles binarios de búsqueda, árboles AVL y árboles de Huffman.

---

## 🚀 Aprendizaje Práctico Experimental (APE)

Espacio dedicado a la resolución de ejercicios y pequeños proyectos donde se modelan problemas reales usando grafos y árboles: representación mediante matrices y listas de adyacencia, cálculo de caminos, construcción de árboles y aplicación de recorridos.

**Competencias desarrolladas:** modelado de problemas con estructuras no lineales, aplicación de algoritmos de búsqueda y recorrido, y pensamiento lógico-computacional.

📎 **Evidencia — APE:** [PEGA_AQUÍ_TU_LINK]

---

## 📖 Aprendizaje Autónomo (AA)

### AA 1 — Investigación sobre Teoría de Grafos

Informe técnico sobre los elementos que componen un grafo (vértices, aristas, tipos de grafos) acompañado de ejemplos prácticos.

📎 **Evidencia — AA 1:** [PEGA_AQUÍ_TU_LINK]

### AA 2 — Árboles en la informática

Ensayo sobre la importancia de los árboles en computación: árboles binarios, árboles AVL, árboles de búsqueda y árboles de Huffman.

📎 **Evidencia — AA 2:** [PEGA_AQUÍ_TU_LINK]

---

## 👨‍🏫 Aprendizaje en Contacto con el Docente (ACD)

### ACD 1 — Exposición y defensa de estructuras de grafos

Sesión enfocada en los distintos tipos de grafos, sus propiedades y sus formas de representación (matrices de adyacencia y listas de adyacencia), con ejemplos aplicados a redes de comunicación y sistemas de transporte.

📎 **Evidencia — ACD 1:** [PEGA_AQUÍ_TU_LINK]

### ACD 2 — Propiedades y recorridos de árboles

Sesión centrada en los conceptos de raíz, hojas, altura y nivel de un árbol, junto con los algoritmos de recorrido (preorden, inorden y postorden).

📎 **Evidencia — ACD 2:** [PEGA_AQUÍ_TU_LINK]

---

## 📝 Evaluación Integradora

Evaluación final que reúne los conocimientos teóricos y prácticos de la unidad: análisis de problemas, selección de la estructura adecuada (grafo o árbol) y aplicación del algoritmo correspondiente.

📎 **Evidencia — Evaluación:** [PEGA_AQUÍ_TU_LINK]

---

## 📊 Conclusiones

Los grafos y los árboles no son solo contenido teórico: son la base de sistemas que se usan todos los días, desde encontrar la ruta más corta hasta organizar el almacenamiento de datos. Comprender cuándo modelar un problema como grafo y cuándo como árbol —y qué algoritmo aplicar en cada caso— es una habilidad central para cualquier persona que se dedique al desarrollo de software o al análisis de sistemas.

---

<p align="center"><i>Unidad 3 completada: de los nodos sueltos a las estructuras que sostienen la conectividad digital.</i></p>

---
[⬅️ Volver al Portafolio](Portafolio-Matematicas-Discretas.md)

