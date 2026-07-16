# STYLEGUIDE

> Este documento define las normas editoriales utilizadas en **The WAS Journey**.
>
> Su objetivo es garantizar que todo el contenido mantenga el mismo estilo, nivel técnico y estructura, independientemente de cuándo se escriba.

---

# Principios generales

## Escribir para comprender, no para memorizar

El objetivo del proyecto no es recopilar definiciones, sino construir modelos mentales sólidos.

Siempre que sea posible:

- explicar el porqué antes que el cómo;
- justificar las decisiones técnicas;
- evitar afirmaciones sin contexto.

---

## HTML primero

Todo el contenido debe fomentar el uso de HTML nativo antes de presentar soluciones basadas en ARIA u otras tecnologías.

Este principio debe reflejarse de forma consistente a lo largo de todo el handbook.

---

## Precisión técnica

Las afirmaciones deben ser técnicamente correctas.

Cuando un concepto admita varias interpretaciones, debe utilizarse la formulación más precisa posible.

Evitar expresiones ambiguas como:

- "ARIA añade semántica."

Preferir:

- "ARIA añade información al árbol de accesibilidad."
- "ARIA complementa la información de accesibilidad."

---

## Evitar simplificaciones engañosas

Es preferible una explicación ligeramente más extensa que una afirmación que pueda inducir a error.

Las simplificaciones solo deben utilizarse cuando no comprometan la comprensión posterior.

---

# Estructura de los documentos del handbook

Cada capítulo debería seguir, siempre que sea posible, la siguiente estructura:

1. Objetivo.
2. Desarrollo del concepto.
3. Ejemplos prácticos.
4. Errores habituales.
5. Ideas clave.
6. Relación con otros capítulos.

---

# Estilo de escritura

## Tono

- Profesional.
- Cercano.
- Didáctico.
- Basado en el razonamiento.

Evitar:

- tono excesivamente académico;
- lenguaje innecesariamente complejo;
- frases motivacionales.

---

## Explicaciones

Siempre que sea posible:

- comenzar por la idea general;
- profundizar progresivamente;
- terminar con una conclusión clara.

---

## Ejemplos

Los ejemplos deben ser:

- pequeños;
- realistas;
- centrados en un único concepto.

Evitar ejemplos excesivamente largos.

---

# Código

## HTML

Utilizar HTML válido y semántico.

Preferir ejemplos pequeños antes que componentes completos.

---

## ARIA

Nunca utilizar ARIA cuando exista una solución HTML equivalente.

Cuando se utilice ARIA, explicar siempre por qué resulta necesaria.

---

## JavaScript

Solo incluir JavaScript cuando sea imprescindible para comprender el concepto.

---

# Terminología

La terminología técnica debe mantenerse en inglés siempre que sea el término utilizado por la especificación.

Ejemplos:

- Accessibility Tree
- Accessible Name
- User Agent
- Screen Reader
- Live Region

Cuando sea necesario, acompañar el término de su traducción la primera vez que aparezca.

---

# Referencias

Las afirmaciones técnicas deben poder respaldarse mediante una especificación oficial o una fuente reconocida.

Preferencia de fuentes:

1. Especificaciones del W3C.
2. WHATWG HTML.
3. WAI-ARIA Authoring Practices.
4. MDN (como documentación de apoyo).
5. IAAP WAS Body of Knowledge.

---

# Academy

Los documentos de la carpeta `academy` complementan cada capítulo del handbook.

Todos deben seguir la misma estructura:

1. Objetivos de aprendizaje.
2. Preguntas tipo WAS.
3. Respuesta correcta.
4. Explicación razonada.
5. Errores habituales.
6. Ideas clave.
7. Autoevaluación.

El objetivo no es memorizar respuestas, sino desarrollar la capacidad de razonamiento necesaria para afrontar preguntas similares a las de la certificación.

---

# Investigación

Los documentos de `research` recogen investigaciones y validaciones técnicas.

No forman parte del handbook.

Una vez consolidado el conocimiento, las conclusiones relevantes podrán incorporarse al handbook.

---

# Principio editorial

Todo contenido nuevo debería responder afirmativamente a estas preguntas:

- ¿Es técnicamente correcto?
- ¿Está respaldado por una fuente fiable?
- ¿Ayuda a comprender el concepto?
- ¿Evita simplificaciones engañosas?
- ¿Encaja con el resto del handbook?
- ¿Aporta información nueva y no duplicada?

Si la respuesta a alguna de estas preguntas es **no**, el contenido deberá revisarse antes de incorporarse al proyecto.