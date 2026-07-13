# Laboratorio

> **Estado:** 🟡 Borrador
>
> El laboratorio es el corazón de *The WAS Journey*. Aquí no buscamos respuestas rápidas, sino comprender cómo funciona realmente la accesibilidad web mediante preguntas, hipótesis, experimentos y evidencia.

---

# Objetivo

Cada vez que surja una duda durante el estudio, la convertiremos en una investigación.

El laboratorio documentará todo el proceso de razonamiento, desde la pregunta inicial hasta la conclusión final.

Nuestro objetivo no es únicamente obtener la respuesta correcta.

Nuestro objetivo es comprender por qué esa respuesta es correcta.

---

# Metodología

Cada investigación seguirá siempre la misma estructura.

## 1. Pregunta

Toda sesión comienza con una única pregunta.

Ejemplos:

- ¿Qué ocurre con un enlace sin `href`?
- ¿Los lectores de pantalla leen el HTML?
- ¿Qué información elimina el Accessibility Tree?
- ¿Puede ARIA modificar el comportamiento de un elemento?

---

## 2. Hipótesis

Antes de consultar documentación, formularemos una hipótesis.

Puede ser correcta o incorrecta.

Lo importante es obligarnos a razonar.

---

## 3. Debate

Analizaremos la hipótesis.

Intentaremos:

- encontrar argumentos a favor;
- encontrar argumentos en contra;
- buscar excepciones;
- identificar casos límite.

---

## 4. Investigación

Solo después acudiremos a las fuentes.

Buscaremos respuestas en:

- Especificaciones.
- Navegadores.
- Tecnologías de asistencia.
- Documentación técnica.
- Profesionales de referencia.

---

## 5. Experimentos

Siempre que sea posible construiremos ejemplos.

No asumiremos comportamientos.

Los comprobaremos.

Por ejemplo:

- inspección del Accessibility Tree;
- pruebas con lectores de pantalla;
- comparación entre navegadores;
- pruebas con teclado;
- validación con herramientas automáticas.

---

## 6. Conclusión

Cada investigación terminará con una conclusión clara.

Debe responder a la pregunta inicial.

Además explicará:

- por qué ocurre;
- qué implicaciones tiene;
- cuándo existen excepciones.

---

## 7. Lecciones aprendidas

Finalmente resumiremos el aprendizaje obtenido.

Estas conclusiones pasarán al documento **05-lecciones-aprendidas.md**.

---

# Plantilla de investigación

Todas las investigaciones seguirán esta plantilla.

```markdown
# Pregunta

## Hipótesis

## Debate

## Investigación

## Experimentos

## Conclusiones

## Referencias

## Lecciones aprendidas
```

---

# Reglas del laboratorio

## Una única pregunta

Nunca investigaremos varias cuestiones al mismo tiempo.

---

## Sin respuestas automáticas

No aceptaremos una respuesta únicamente porque aparezca en un artículo, una IA o una presentación.

Toda afirmación deberá poder justificarse.

---

## Buscar contraejemplos

Cuando creamos haber encontrado una respuesta, intentaremos demostrar que es falsa.

Si resiste ese intento, nuestra confianza aumentará.

---

## Diferenciar especificación e implementación

No confundiremos nunca:

- lo que define una especificación;
- lo que implementa un navegador;
- lo que interpreta una tecnología de asistencia.

Las tres cosas pueden diferir.

---

## Documentar también los errores

Las hipótesis incorrectas también aportan conocimiento.

Documentarlas evitará repetir los mismos errores en el futuro.

---

# Ejemplos de investigaciones

Algunas investigaciones previstas:

- ¿Qué ocurre con un `<a>` sin `href`?
- ¿Por qué un `<button>` es diferente de un `<div role="button">`?
- ¿Qué añade realmente `role="button"`?
- ¿Cómo construye el navegador el Accessibility Tree?
- ¿Qué información ignora un lector de pantalla?
- ¿Qué ocurre cuando usamos `aria-hidden`?
- ¿Puede un elemento tener varios roles?
- ¿Qué diferencia existe entre nombre, rol y estado?
- ¿Qué ocurre cuando modificamos dinámicamente el DOM?
- ¿Cómo afectan las Shadow DOM a la accesibilidad?

---

# Criterios de calidad

Una investigación solo se considerará finalizada cuando:

- exista una respuesta clara;
- la respuesta esté respaldada por fuentes fiables;
- se hayan realizado experimentos cuando sea posible;
- se hayan identificado excepciones;
- la conclusión pueda explicarse con nuestras propias palabras.

---

# Resultado esperado

Con el paso del tiempo, este laboratorio se convertirá en un registro del proceso de aprendizaje.

No solo documentará respuestas.

Documentará cómo llegamos a ellas.

Ese razonamiento será, probablemente, el activo más valioso de todo el proyecto.

---

> **No memorices las respuestas. Aprende a formular las preguntas correctas.**