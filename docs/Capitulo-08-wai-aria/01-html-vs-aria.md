# HTML vs ARIA

## Objetivo

Comprender por qué HTML y ARIA no son tecnologías equivalentes y por qué los elementos HTML nativos deben ser siempre la primera opción para construir interfaces accesibles.

---

## HTML y ARIA no tienen la misma responsabilidad

Uno de los errores más habituales al comenzar a estudiar accesibilidad es pensar que HTML y ARIA persiguen el mismo objetivo.

No es así.

Aunque ambos participan en la construcción del árbol de accesibilidad (*Accessibility Tree*), cada uno tiene una responsabilidad diferente.

### HTML

HTML define la estructura de la interfaz y proporciona capacidades nativas que el navegador implementa de forma automática.

Entre ellas:

- Semántica.
- Comportamiento.
- Integración con la plataforma web.

Por ejemplo, un elemento `<button>`:

- tiene un rol implícito de botón;
- puede recibir el foco;
- responde correctamente al teclado y al puntero;
- puede asociarse a un formulario mediante el atributo `form`;
- participa en la validación de formularios;
- expone toda esta información al árbol de accesibilidad.

Todo ello sin necesidad de implementar lógica adicional.

---

### ARIA

ARIA no sustituye a HTML.

Su objetivo es complementar la información que el navegador expone al árbol de accesibilidad cuando HTML, por sí solo, no puede expresar correctamente el propósito, el estado o las relaciones de un componente.

ARIA permite definir, entre otros aspectos:

- Roles.
- Estados.
- Propiedades accesibles.

Un ejemplo es:

```html
<div role="alert">
    Error al guardar los cambios.
</div>
```

HTML no dispone de un elemento nativo equivalente para representar una alerta dinámica. En este caso, `role="alert"` permite que el navegador exponga ese contenido como una región activa (*live region*) de alta prioridad para las tecnologías de asistencia.

---

## HTML primero

Existe una regla que debería guiar el desarrollo de cualquier interfaz accesible:

> Si existe un elemento HTML nativo adecuado, debe utilizarse antes que una solución basada en ARIA.

La razón no es únicamente la semántica.

Los elementos HTML nativos también proporcionan comportamiento e integración con la plataforma que ARIA, por sí sola, no puede ofrecer.

---

## Un rol no cambia la naturaleza del elemento

Asignar un rol mediante ARIA no convierte un elemento en otro elemento HTML.

Por ejemplo:

```html
<div role="button" tabindex="0">
    Guardar
</div>
```

Puede comunicar al árbol de accesibilidad que el elemento debe tratarse como un botón.

Sin embargo, no adquiere automáticamente todas las capacidades de un `<button>` nativo.

El desarrollador deberá implementar manualmente el comportamiento esperado y, aun así, es posible que no alcance el mismo nivel de integración que proporciona el navegador.

---

## Ideas clave

- HTML y ARIA tienen responsabilidades diferentes.
- HTML debe ser siempre la primera opción.
- ARIA complementa a HTML; no lo sustituye.
- Un rol no transforma un elemento HTML en otro elemento nativo.
- Los elementos HTML nativos ofrecen semántica, comportamiento e integración con la plataforma.

---

## Próximo capítulo

En este punto surge una pregunta natural:

> Si HTML y ARIA contribuyen al árbol de accesibilidad, ¿cómo construye realmente el navegador ese árbol y cómo llega esa información a un lector de pantalla?

Ese será el siguiente paso del viaje.