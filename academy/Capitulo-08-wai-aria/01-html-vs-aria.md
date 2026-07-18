# Academy · 05 · HTML y ARIA

> Este documento complementa `docs/05-html-y-aria.md`.
>
> Su objetivo no es memorizar respuestas, sino entrenar el razonamiento necesario para afrontar preguntas similares a las de la certificación **IAAP WAS**.

---

# Objetivos de aprendizaje

Al finalizar este capítulo deberías ser capaz de:

- Explicar por qué HTML y ARIA tienen responsabilidades diferentes.
- Justificar por qué siempre debe preferirse HTML nativo cuando exista un elemento adecuado.
- Diferenciar entre la semántica HTML y la información de accesibilidad proporcionada por ARIA.
- Comprender qué aporta realmente un `role`.
- Identificar cuándo el uso de ARIA está justificado.

---

# Pregunta 1

## ¿Cuál de las siguientes afirmaciones es la más correcta?

**A.** ARIA puede utilizarse para convertir cualquier elemento HTML en su equivalente nativo.

**B.** Los elementos HTML nativos suelen ofrecer semántica y comportamiento que ARIA no puede proporcionar por sí sola.

**C.** Si un elemento tiene el `role` correcto, su comportamiento será equivalente al de un elemento HTML nativo.

**D.** HTML y ARIA tienen el mismo propósito; la diferencia principal es la sintaxis.

### ✅ Respuesta correcta

**B**

### Explicación

Los elementos HTML nativos proporcionan de forma integrada:

- Semántica.
- Comportamiento.
- Integración con la plataforma.

ARIA únicamente complementa la información que se expone al árbol de accesibilidad.

---

# Pregunta 2

## ¿Cuál es el principal objetivo de ARIA?

**A.** Sustituir HTML en aplicaciones JavaScript.

**B.** Añadir información de accesibilidad cuando HTML no puede expresar correctamente el propósito, el estado o las relaciones de un componente.

**C.** Mejorar automáticamente la accesibilidad de cualquier elemento HTML.

**D.** Convertir elementos genéricos en elementos HTML nativos.

### ✅ Respuesta correcta

**B**

### Explicación

ARIA nace para cubrir casos donde HTML no dispone de un mecanismo nativo adecuado.

No sustituye HTML ni implementa automáticamente el comportamiento de los elementos.

---

# Pregunta 3

## ¿Cuál de las siguientes afirmaciones describe mejor la relación entre HTML y ARIA?

**A.** HTML y ARIA son tecnologías equivalentes.

**B.** HTML define la interfaz; ARIA únicamente añade estilos visuales.

**C.** HTML proporciona estructura, semántica y comportamiento; ARIA complementa la información de accesibilidad cuando es necesario.

**D.** ARIA debe utilizarse siempre que se desarrolla una SPA.

### ✅ Respuesta correcta

**C**

### Explicación

HTML y ARIA no compiten entre sí.

HTML debe ser siempre la primera opción.

ARIA únicamente complementa la información accesible cuando HTML no puede expresar correctamente el significado, estado o relaciones de un componente.

---

# Pregunta 4

## ¿Qué ocurre al asignar `role="button"` a un `<div>`?

**A.** Se convierte en un elemento `<button>`.

**B.** Adquiere automáticamente el mismo comportamiento que un botón nativo.

**C.** El árbol de accesibilidad lo expondrá con el rol de botón, pero el comportamiento deberá implementarse manualmente.

**D.** El navegador sustituye el elemento por un `<button>` durante el renderizado.

### ✅ Respuesta correcta

**C**

### Explicación

Un rol ARIA no modifica la naturaleza del elemento HTML.

El desarrollador continúa siendo responsable de implementar el comportamiento esperado.

---

# Pregunta 5

## ¿Cuál de las siguientes afirmaciones sobre `role="alert"` es la más correcta?

**A.** Hace que el navegador muestre automáticamente un cuadro de diálogo.

**B.** Convierte un `<div>` en un elemento HTML especializado.

**C.** Permite que el navegador exponga el contenido como una región activa (*live region*) de alta prioridad para las tecnologías de asistencia.

**D.** Tiene el mismo efecto que utilizar `<strong>`.

### ✅ Respuesta correcta

**C**

### Explicación

`role="alert"` comunica al navegador que ese contenido debe exponerse como una alerta dentro del árbol de accesibilidad.

Las tecnologías de asistencia podrán anunciar el cambio al usuario cuando corresponda.

---

# Pregunta 6

## ¿Cuál es la mejor práctica cuando existe un elemento HTML nativo adecuado?

**A.** Utilizar siempre un `<div>` con ARIA para tener mayor flexibilidad.

**B.** Utilizar el elemento HTML nativo.

**C.** Utilizar ARIA únicamente porque mejora el SEO.

**D.** Ambas opciones son equivalentes.

### ✅ Respuesta correcta

**B**

### Explicación

Los elementos HTML nativos ofrecen capacidades que ARIA no puede proporcionar por sí sola.

Esta es una de las reglas fundamentales de la accesibilidad web.

---

# Errores habituales

- Pensar que ARIA sustituye HTML.
- Creer que un `role` cambia la naturaleza del elemento.
- Suponer que ARIA implementa comportamiento automáticamente.
- Utilizar ARIA cuando ya existe un elemento HTML adecuado.

---

# Ideas clave

- HTML primero.
- ARIA complementa; no sustituye.
- Un rol no convierte un elemento en otro elemento HTML.
- Los elementos HTML nativos proporcionan semántica, comportamiento e integración con la plataforma.
- Antes de añadir ARIA, pregúntate siempre si HTML ya resuelve el problema.

---

# Autoevaluación

Si puedes responder con tus propias palabras a las siguientes preguntas sin consultar el handbook, puedes considerar este capítulo superado:

- ¿Por qué HTML debe ser la primera opción?
- ¿Qué problema resuelve realmente ARIA?
- ¿Qué diferencia existe entre un `<button>` y un `<div role="button">`?
- ¿Qué aporta `role="alert"` que HTML no ofrece de forma nativa?
- ¿Por qué un rol ARIA no convierte un elemento en otro elemento HTML?