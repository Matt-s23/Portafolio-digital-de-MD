<div align="center">

# PORTAFOLIO DE MATEMÁTICAS DISCRETAS

### Universidad Nacional de Loja

![Banner](https://univercimas.com/wp-content/uploads/2021/04/Universidad-Nacional-de-Loja-UNL.png)

<br>

<img src="https://img.shields.io/badge/MATEMÁTICAS-DISCRETAS-0d6efd?style=for-the-badge&labelColor=0b1120" />
<img src="https://img.shields.io/badge/GITHUB-PORTAFOLIO-181717?style=for-the-badge&logo=github" />
<img src="https://img.shields.io/badge/UNIDAD-1_ACTIVA-success?style=for-the-badge" />

---

## Información Académica

| Campo | Información |
|:---|:---|
| Estudiante | **Matias Santiago Calva Gonzalez** |
| Docente | **Ing. Mario Enrique Cueva** |
| Carrera | **Computación** |
| Asignatura | **Matemáticas Discretas** |
| Ciclo | **Primer Ciclo** |
| Año Lectivo | **2026** |

---

> *"La lógica es la base del razonamiento computacional."*

</div>

---

# ÍNDICE GENERAL

<details open>
<summary><b>Navegación del Portafolio</b></summary>

<br>

## Unidad 1 — Lógica Proposicional

### Contenido Teórico
- [1.1 ¿Qué es una proposición?](#11--qué-es-una-proposición)
- [1.2 Tipos de proposiciones](#12--tipos-de-proposiciones)
- [1.3 Conectores lógicos](#13--conectores-lógicos)
- [1.4 Tablas de verdad](#14--tablas-de-verdad)
- [1.5 Leyes proposicionales](#15--leyes-proposicionales)
- [1.6 Reglas de inferencia](#16--reglas-de-inferencia)

### Ejercicios Resueltos
- [Ejercicio 1 — Traducción de lenguaje natural a simbólico](#ejercicio-1--traducción-de-lenguaje-natural-a-simbólico)
- [Ejercicio 2 — Construcción de tablas de verdad](#ejercicio-2--construcción-de-tablas-de-verdad)
- [Ejercicio 3 — Tautologías, contradicciones y contingencias](#ejercicio-3--tautologías-contradicciones-y-contingencias)
- [Ejercicio 4 — Aplicación de leyes proposicionales](#ejercicio-4--aplicación-de-leyes-proposicionales)
- [Ejercicio 5 — Validación de argumentos](#ejercicio-5--validación-de-argumentos)

### Ejercicio Aplicado
- [Caso real o cotidiano](#ejercicio-aplicado)

### Reflexión Personal
- [¿Qué fue lo más difícil de entender?](#qué-fue-lo-más-difícil-de-entender)
- [¿Qué tema comprendí mejor?](#qué-tema-comprendí-mejor)
- [¿Cómo puedo aplicar la lógica en mi carrera?](#cómo-puedo-aplicar-la-lógica-en-mi-carrera)

### Otras Unidades
- [Unidad 2 — No habilitado](#unidad-2--no-habilitado)
- [Unidad 3 — No habilitado](#unidad-3--no-habilitado)

</details>

---

# UNIDAD 1 — LÓGICA PROPOSICIONAL

## Introducción

La lógica proposicional es una de las bases fundamentales de las matemáticas discretas y del razonamiento computacional. Permite representar información mediante símbolos y analizar si un razonamiento es válido o incorrecto.

Actualmente se aplica en áreas como desarrollo de software, inteligencia artificial, seguridad informática, redes computacionales, bases de datos y electrónica digital.

---

## 1.1 — ¿Qué es una proposición?

Una **proposición** es un enunciado declarativo que puede clasificarse como **verdadero** o **falso**, nunca ambos a la vez.

### Ejemplos de proposiciones

| Enunciado | Valor |
|---|---|
| 7 es un número primo | Verdadero |
| 2 + 2 = 5 | Falso |
| Python es un sistema operativo | Falso |

### Expresiones que NO son proposiciones

| Expresión | Motivo |
|---|---|
| ¿Cómo estás? | Pregunta |
| Guarda el archivo | Orden |
| Ojalá funcione | Deseo |

> Toda proposición debe poseer un valor de verdad definido.

---

## 1.2 — Tipos de proposiciones

Las proposiciones pueden clasificarse en **simples** y **compuestas**.

### Proposiciones simples

No contienen conectores lógicos. Son la unidad mínima de análisis.

Ejemplos:
- `p` : El servidor está activo
- `q` : El usuario inició sesión

### Proposiciones compuestas

Se forman combinando proposiciones simples mediante conectores lógicos.

Ejemplos: `p ∧ q`, `p → q`, `¬p`

| Tipo | Característica |
|---|---|
| Simples | No pueden dividirse en partes más pequeñas |
| Compuestas | Contienen uno o más conectores lógicos |

---

## 1.3 — Conectores lógicos

Los **conectores lógicos** permiten relacionar proposiciones para formar expresiones compuestas.

| Símbolo | Nombre | Lectura | Descripción |
|---|---|---|---|
| ¬ | Negación | "No" | Invierte el valor de verdad |
| ∧ | Conjunción | "Y" | Verdadero solo si ambas son verdaderas |
| ∨ | Disyunción | "O" | Falso solo si ambas son falsas |
| → | Condicional | "Si... entonces" | Falso solo cuando el antecedente es V y el consecuente F |
| ↔ | Bicondicional | "Si y solo si" | Verdadero cuando ambas tienen el mismo valor |

| Lógica | Programación |
|---|---|
| ¬p | !p |
| p ∧ q | p && q |
| p ∨ q | p \|\| q |

---

## 1.4 — Tablas de verdad

Las **tablas de verdad** permiten analizar todas las combinaciones posibles de valores de una expresión lógica. Con `n` variables, se generan `2ⁿ` filas.

| Paso | Descripción |
|---|---|
| 1 | Identificar las variables |
| 2 | Calcular el número de filas con 2ⁿ |
| 3 | Construir las columnas de izquierda a derecha |
| 4 | Resolver operadores de menor a mayor precedencia |
| 5 | Obtener el resultado final |

### Tabla básica para p y q

| p | q | ¬p | p ∧ q | p ∨ q | p → q | p ↔ q |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| V | V | F | V | V | V | V |
| V | F | F | F | V | F | F |
| F | V | V | F | V | V | F |
| F | F | V | F | F | V | V |

### Clasificación de expresiones

| Tipo | Resultado | Ejemplo |
|---|---|---|
| Tautología | Siempre verdadero | p ∨ ¬p |
| Contradicción | Siempre falso | p ∧ ¬p |
| Contingencia | Valores mixtos | p → q |

---

## 1.5 — Leyes proposicionales

Las **leyes proposicionales** permiten simplificar o transformar expresiones lógicas sin alterar su significado.

| Ley | Equivalencia |
|---|---|
| Doble negación | ¬(¬p) ≡ p |
| De Morgan (conjunción) | ¬(p ∧ q) ≡ ¬p ∨ ¬q |
| De Morgan (disyunción) | ¬(p ∨ q) ≡ ¬p ∧ ¬q |
| Implicación material | p → q ≡ ¬p ∨ q |
| Conmutativa (∧) | p ∧ q ≡ q ∧ p |
| Conmutativa (∨) | p ∨ q ≡ q ∨ p |
| Absorción | p ∧ (p ∨ q) ≡ p |
| Identidad | p ∧ V ≡ p |

---

## 1.6 — Reglas de inferencia

Las **reglas de inferencia** permiten obtener conclusiones válidas a partir de premisas conocidas.

**Modus Ponens:** Si p → q y p, entonces ∴ q

**Modus Tollens:** Si p → q y ¬q, entonces ∴ ¬p

**Silogismo Hipotético:** Si p → q y q → r, entonces ∴ p → r

**Adición:** Si p, entonces ∴ p ∨ q

**Simplificación:** Si p ∧ q, entonces ∴ p

---

# EJERCICIOS RESUELTOS

---

## Ejercicio 1 — Traducción de lenguaje natural a simbólico

<details open>
<summary><b>Ver ejercicio</b></summary>

<br>

<<img width="938" height="1346" alt="WhatsApp Image 2026-05-13 at 7 16 04 PM" src="https://github.com/user-attachments/assets/098b9503-cba7-4709-96de-d0049ab6a295" />

</details>

---

## Ejercicio 2 — Construcción de tablas de verdad

<details>
<summary><b>Ver ejercicio</b></summary>

<br>

<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/71bde926-db9c-4585-b3b4-a25ee4b93a1c" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/7fe0a8fe-3d44-4053-901c-359fd82a52ca" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/4d46cfbf-1601-45ae-aaab-ce823218cdca" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/4dc5a7bb-99ad-4f8b-beb7-42da3dcf262d" />

</details>

---

## Ejercicio 3 — Tautologías, contradicciones y contingencias

<details>
<summary><b>Ver ejercicio</b></summary>

<br>

<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/d0d7223b-b81f-4e72-8914-27ff43478e56" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/fb8460eb-2034-46e5-b140-6d8cb11243fb" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/409cbaac-6999-4799-ab73-362fe79d79b2" />

</details>

---

## Ejercicio 4 — Aplicación de leyes proposicionales

<details>
<summary><b>Ver ejercicio</b></summary>

<br>

<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/10c6a716-33b6-4e9a-8990-061d33cb5219" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/a3df0c30-a5e7-45c7-8f87-a40e04c35ca2" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/edbd43aa-1183-412e-a4c5-94149d7faae8" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/480708b0-1902-4cd5-8009-6ffc9edf683c" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/441dca26-a92e-4a80-9c8b-ce0341bd710c" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/0c2c279f-dc7f-4c44-8ae8-0875f76a1c79" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/157a6365-6e46-48fb-85e8-a27cac2641b6" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/e62157e1-4e08-403e-a01f-a68dbadaa78d" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/0934b928-498d-4d19-b859-603442f1365e" />

</details>

---

## Ejercicio 5 — Validación de argumentos

<details>
<summary><b>Ver ejercicio</b></summary>

<br>

<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/f01f352e-f925-4a2e-9e48-c6c7d87062a1" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/54f8832f-387d-497d-aa45-c34fb887e6bc" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/d0f3083e-b95b-47af-bfe2-8f857e371fc1" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/ba1e7bfa-3464-4142-a85a-51d7be3906b9" />
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/d46861a8-5275-41b2-98aa-82ccd27678fa" />


</details>

---

# EJERCICIO APLICADO

<details open>
<summary><b>Caso real: Sistema de acceso universitario</b></summary>

<br>

## Problema planteado

Una plataforma virtual universitaria permite el acceso a un examen **únicamente si** el estudiante ha iniciado sesión **y** posee matrícula activa. Si alguna condición no se cumple, el sistema bloqueará el acceso automáticamente.

---

## Definición de proposiciones

| Variable | Significado |
|---|---|
| p | El estudiante inició sesión |
| q | El estudiante tiene matrícula activa |
| r | El estudiante puede acceder al examen |

---

## Expresión simbólica

(p ∧ q) → r

---

## Análisis lógico

| p | q | p ∧ q | Resultado (r) |
|:---:|:---:|:---:|:---|
| V | V | V | Puede acceder al examen |
| V | F | F | No puede acceder (sin matrícula) |
| F | V | F | No puede acceder (sin sesión) |
| F | F | F | No puede acceder |

---

## Conclusión

La lógica proposicional permite representar situaciones reales de manera precisa. En este caso se modela exactamente cómo un sistema informático toma decisiones mediante condiciones lógicas combinadas, lo que es la base de cualquier sistema de autenticación y autorización en software.

</details>

---

# REFLEXIÓN PERSONAL

---

<details open>
<summary><b>¿Qué fue lo más difícil de entender?</b></summary>

<br>

Lo más difícil fue comprender las **leyes proposicionales** y las **reglas de inferencia**, ya que al principio no quedaba claro cómo aplicarlas paso a paso sin cometer errores en el proceso de deducción.

</details>

---

<details>
<summary><b>¿Qué tema comprendí mejor?</b></summary>

<br>

El tema que comprendí mejor fueron las **tablas de verdad**, porque su estructura sistemática permite analizar todas las combinaciones posibles de manera ordenada y verificable.

</details>

---

<details>
<summary><b>¿Cómo puedo aplicar la lógica en mi carrera?</b></summary>

<br>

La lógica proposicional tiene aplicaciones directas en mi carrera de Computación:

- **Desarrollo de software**: estructuras condicionales y validaciones
- **Algoritmos**: análisis de condiciones y toma de decisiones
- **Bases de datos**: consultas con condiciones lógicas (AND, OR, NOT)
- **Inteligencia artificial**: sistemas expertos y razonamiento automático
- **Ciberseguridad**: sistemas de control de acceso y autenticación

</details>

---

# UNIDAD 2 — NO HABILITADO

<div align="center">

⚠️ Contenido aún no disponible

</div>

---

# UNIDAD 3 — NO HABILITADO

<div align="center">

⚠️ Contenido aún no disponible

</div>

---

# CONCLUSIÓN GENERAL

La lógica proposicional constituye una herramienta fundamental para el razonamiento formal y el desarrollo computacional. Gracias a ella es posible analizar situaciones complejas, validar argumentos y desarrollar sistemas eficientes y seguros. Su estudio es indispensable para cualquier profesional del área de la computación.

---

<div align="center">

# Universidad Nacional de Loja

### Matemáticas Discretas · Portafolio Académico · 2026

<img src="https://img.shields.io/badge/PORTAFOLIO-COMPLETADO-success?style=for-the-badge" />

<br>

Elaborado en GitHub Markdown · Diseño académico interactivo

</div>

</div>
