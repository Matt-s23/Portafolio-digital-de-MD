[⬅️ Volver al Portafolio](Portafolio-Matematicas-Discretas.md)
---

<h1 align="center">⚡ UNIDAD 2 · Álgebra de Boole, Karnaugh y Diseño Lógico</h1>
<p align="center"><i>Del razonamiento simbólico al circuito físico</i></p>

---

## 🧭 Contenido de esta página

| Sección | Tema |
|---|---|
| 📘 Fase 1 y 2 | Álgebra de Boole: leyes y simplificación algebraica |
| 📘 Fase 3 y 4 | Mapas de Karnaugh (2, 3 y 4 variables) |
| 📘 Fase 5 y 6 | Teoremas avanzados, compuertas universales y proyecto integrador |
| 📖 AA | Aprendizaje Autónomo |
| 👨‍🏫 ACD | Sesiones con el docente |

> 📎 **Nota:** solo pega el enlace de Google Drive donde tengas guardada la evidencia de cada fase en el marcador `[PEGA_AQUÍ_TU_LINK]`.

---

## 📘 Fase 1 y 2 — Álgebra de Boole y simplificación algebraica

**Semanas de trabajo:** 6-7 · **Periodo:** mayo 2026

El punto de partida fue el conjunto de leyes que gobiernan el álgebra booleana: conmutatividad, asociatividad, distributividad, identidad, complemento, idempotencia, absorción, consenso y las leyes de De Morgan. Con esas herramientas, cualquier expresión booleana —sin importar cuántos términos tenga— puede reducirse a una forma mínima sin alterar su comportamiento lógico.

La metodología de trabajo siguió tres momentos: explicación teórica de cada ley con demostración simbólica, práctica guiada identificando qué ley aplicar según el patrón de la expresión, y verificación cruzada comparando la tabla de verdad de la expresión original contra la de su versión simplificada.

Se resolvió una progresión de 5 ejercicios, desde expresiones básicas de 2 variables hasta expresiones complejas de 7 variables, cada uno validado construyendo su tabla de verdad completa.

📎 **Evidencia — Fase 1 y 2:** https://drive.google.com/drive/u/1/folders/1lTuiBrIe-XZo8t3ibafezVcZdkmKDXtC

---

## 📘 Fase 3 y 4 — Mapas de Karnaugh

El Mapa de Karnaugh reemplaza el álgebra simbólica por una lectura visual: cada celda representa una combinación posible de variables, y las celdas adyacentes que comparten el valor **1** pueden agruparse en bloques de 1, 2, 4 u 8 celdas. Cuanto más grande el grupo, más se reduce la expresión final.

El recorrido de aprendizaje cubrió:

- Construcción de mapas para **2, 3 y 4 variables**.
- Identificación de adyacencias válidas (incluyendo los bordes, que en un K-Map "se envuelven").
- Conversión entre **formas canónicas**: suma de productos (SOP) y producto de sumas (POS), usando mintérminos (m) y maxtérminos (M).
- Un caso aplicado (sistema de alarma / control de acceso) resuelto siguiendo la cadena completa: problema → tabla de verdad → mapa de Karnaugh → expresión simplificada → circuito lógico, verificado también por vía algebraica.
- Una comparación crítica entre el método algebraico y el método gráfico:

| Criterio | Álgebra de Boole | Mapas de Karnaugh |
|---|---|---|
| Curva de aprendizaje | Requiere memorizar leyes | Más intuitivo, visual |
| Riesgo de error | Alto en expresiones largas | Bajo hasta 4-5 variables |
| Escalabilidad | Funciona con cualquier número de variables | Pierde practicidad después de 5-6 variables |

Se cerró la fase con 5 ejercicios individuales de minimización, cada uno verificado con una herramienta de software de comprobación booleana.

📎 **Evidencia — Fase 3 y 4:** https://drive.google.com/drive/u/1/folders/1B6wFZ9LyLFTd03WxwNLew8qExL5F8PTi

---

## 📘 Fase 5 y 6 — Teoremas avanzados, compuertas universales y proyecto integrador

### 🔎 Investigación autónoma: tres teoremas adicionales

**1. Teorema del Consenso Dual** — versión del teorema del consenso para expresiones en producto de sumas (POS): `(A+B)·(A'+C)·(B+C) = (A+B)·(A'+C)`. En hardware, este ahorro elimina una compuerta OR completa del circuito.

**2. Leyes de De Morgan aplicadas a software** — además de su uso en circuitos, permiten reescribir condicionales complejos de programación en una forma más legible:
```python
# Original
if not (status == "active" and points > 100):
    ...
# Aplicando De Morgan
if status != "active" or points <= 100:
    ...
```

**3. Teorema de Expansión de Shannon** — permite descomponer cualquier función booleana aislando una variable de control: `F = X1·F(1,...) + X1'·F(0,...)`. La variable aislada se comporta como la línea de selección de un multiplexor 2 a 1, principio base de cómo las FPGAs implementan lógica programable.

### 🔌 Compuertas universales (NAND / NOR)

Práctica de implementación de funciones booleanas usando exclusivamente compuertas NAND o NOR, demostrando por qué se consideran "compuertas universales".

### 🌱 Ensayo: optimización lógica y sostenibilidad tecnológica

> Cada compuerta eliminada de un circuito mediante simplificación booleana representa menos silicio fabricado, menos energía consumida y, a escala industrial, un impacto ambiental medible — en lo económico (menos componentes que fabricar), lo energético (menos transistores activos) y lo ambiental (menos residuo electrónico).

### ➕ Proyecto integrador: sumador binario de 1 bit

Diseño de un sumador de 1 bit aplicando de forma encadenada todo lo aprendido: tabla de verdad de las 8 combinaciones de A, B y Cin → funciones booleanas de S y Cout → simplificación doble (Karnaugh y verificación algebraica) → circuito lógico final con compuertas XOR, AND y OR.

📎 **Evidencia — Fase 5 y 6:** https://drive.google.com/drive/u/1/folders/1E7e0M4O5C6Asd757s3378Zn1UQKAh7Ay

---

## 📖 Aprendizaje Autónomo (AA)

El trabajo autónomo permitió profundizar en los teoremas avanzados, resolver ejercicios adicionales de simplificación y documentar el ensayo reflexivo sobre sostenibilidad tecnológica.

📎 **Evidencia — AA:** https://drive.google.com/drive/u/1/folders/1XfG42nAYO6w5A2mX5zslRMUUDZTQSRq_

---

## 👨‍🏫 Aprendizaje en Contacto con el Docente (ACD)

Registro de las sesiones guiadas por el docente durante esta unidad.

📎 **Evidencia — ACD:** https://drive.google.com/drive/u/1/folders/1BdfN6eDr70FEu9vaieDYMK7Vvv3npZL4

---

<p align="center"><i>Unidad 2 completada: del símbolo booleano al circuito físico, pasando por la sostenibilidad del diseño digital.</i></p>

---
[⬅️ Volver al Portafolio](Portafolio-Matematicas-Discretas.md)
