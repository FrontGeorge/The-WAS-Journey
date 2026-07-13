# Conceptos fundamentales

> **Estado:** 🟡 Borrador
>
> Este documento define los conceptos fundamentales sobre los que se construirá el resto del proyecto. No pretende explicarlos en profundidad, sino establecer un mapa de conocimiento y las relaciones entre ellos.

---

# Objetivos de aprendizaje

Al finalizar esta parte del proyecto deberíamos ser capaces de:

- Comprender cómo funciona la plataforma web desde el punto de vista de la accesibilidad.
- Diferenciar HTML, DOM, Accessibility Tree y tecnologías de asistencia.
- Entender el papel de la semántica en la Web.
- Comprender cuándo utilizar HTML nativo y cuándo es necesario recurrir a ARIA.
- Desarrollar un modelo mental sólido sobre cómo viaja la información desde nuestro código hasta el usuario.

---

# Modelo mental

Toda la accesibilidad web puede entenderse siguiendo el siguiente flujo:

```text
                 Plataforma Web
                        │
        ┌───────────────┴───────────────┐
        │                               │
      HTML                             CSS
        │
        ▼
       DOM
        │
        ▼
Accessibility Tree
        │
        ▼
Accessibility APIs
        │
        ▼
Tecnologías de asistencia
        │
        ▼
        Usuario
```

Este diagrama será una referencia constante durante todo el proyecto.

Nuestro objetivo será comprender qué ocurre en cada paso del proceso y cómo afecta cualquier decisión que tomemos durante el desarrollo.

---

# Conceptos fundamentales

## 1. ¿Qué es la accesibilidad web?

Antes de estudiar tecnologías o estándares, debemos responder una pregunta aparentemente sencilla:

> ¿Qué significa realmente que una interfaz sea accesible?

Estudiaremos:

- Inclusión.
- Barreras.
- Discapacidad.
- Diseño universal.
- Accesibilidad y usabilidad.
- Accesibilidad como característica de calidad.

---

## 2. La plataforma web

La accesibilidad no es una capa añadida sobre una aplicación.

Forma parte de la propia plataforma web.

Comprenderemos cómo se relacionan:

- HTML.
- CSS.
- JavaScript.
- Navegadores.
- Especificaciones.

---

## 3. HTML semántico

HTML no solo define la estructura visual de un documento.

También proporciona significado.

Responderemos preguntas como:

- ¿Qué significa que un elemento sea semántico?
- ¿Por qué `<button>` y `<div>` no son equivalentes?
- ¿Qué información aporta HTML al navegador?

---

## 4. El DOM

Analizaremos:

- Qué representa realmente el DOM.
- Cómo lo construye el navegador.
- Qué relación guarda con el documento HTML.
- Qué papel desempeña JavaScript.

---

## 5. El Accessibility Tree

Este será uno de los capítulos más importantes del proyecto.

Comprenderemos:

- Qué es.
- Cómo se genera.
- Qué información contiene.
- Qué información descarta.
- Cómo lo modifica HTML.
- Cómo lo modifica ARIA.

Gran parte de las dudas habituales sobre accesibilidad desaparecen cuando se comprende correctamente este concepto.

---

## 6. Accessibility APIs

Los navegadores no se comunican directamente con las tecnologías de asistencia.

Utilizan las APIs de accesibilidad del sistema operativo.

Estudiaremos:

- UI Automation (Windows)
- AX API (macOS)
- ATK / AT-SPI (Linux)

Comprenderemos qué información reciben estas APIs y cuál no.

---

## 7. Tecnologías de asistencia

Analizaremos cómo interactúan con la información proporcionada por el navegador.

Entre otras:

- Lectores de pantalla.
- Magnificadores.
- Control por voz.
- Dispositivos alternativos de entrada.

Nuestro objetivo será comprender cómo utilizan el Accessibility Tree.

---

## 8. Navegadores

Los navegadores implementan las especificaciones.

Pero no siempre de la misma forma.

Estudiaremos:

- Chromium.
- Firefox.
- Safari.

Prestando especial atención a las diferencias de implementación que afectan a la accesibilidad.

---

## 9. WAI-ARIA

ARIA no sustituye a HTML.

Nuestro objetivo será comprender:

- Qué problema intenta resolver.
- Cuándo debe utilizarse.
- Cuándo no debe utilizarse.
- Qué limitaciones tiene.

Nuestro principio será siempre:

> **HTML nativo primero. ARIA cuando sea necesario.**

---

## 10. WCAG

Solo cuando comprendamos el funcionamiento de la plataforma estudiaremos las WCAG.

No memorizararemos criterios.

Intentaremos responder:

- ¿Qué problema resuelve cada criterio?
- ¿Qué usuarios protege?
- ¿Cómo puede verificarse?

---

# Relaciones entre conceptos

Durante todo el proyecto insistiremos en las relaciones entre los distintos conceptos.

Por ejemplo:

- HTML influye en el Accessibility Tree.
- ARIA modifica el Accessibility Tree.
- JavaScript puede modificar el DOM.
- Los lectores de pantalla no interpretan directamente el HTML.
- Las WCAG describen requisitos, no implementaciones.
- La semántica y el comportamiento son conceptos diferentes.

Comprender estas relaciones será más importante que memorizar cualquier definición.

---

# Errores habituales

Intentaremos evitar algunos errores muy frecuentes.

- Confundir HTML con el DOM.
- Confundir el DOM con el Accessibility Tree.
- Pensar que ARIA añade comportamiento.
- Pensar que los lectores de pantalla leen directamente el HTML.
- Memorizar WCAG sin comprender el problema que resuelven.
- Sustituir HTML nativo por ARIA sin necesidad.

---

# Preguntas que responderemos

A lo largo de este proyecto resolveremos preguntas como:

- ¿Qué es realmente la accesibilidad?
- ¿Qué hace un navegador cuando interpreta HTML?
- ¿Qué información llega al Accessibility Tree?
- ¿Cómo obtiene un lector de pantalla esa información?
- ¿Cuándo debe utilizarse ARIA?
- ¿Qué ocurre cuando modificamos un rol?
- ¿Qué diferencia existe entre semántica y comportamiento?

---

# Referencias principales

Este documento se desarrollará utilizando principalmente:

## Especificaciones

- W3C
- WHATWG
- IAAP
- EN 301 549

## Documentación técnica

- WAI-ARIA Authoring Practices Guide (APG)
- MDN Web Docs
- web.dev

## Profesionales de referencia

- Olga Carreras
- Adrian Roselli
- Steve Faulkner
- Léonie Watson
- Sarah Higley
- WebAIM
- TPGi

---

# Próximos pasos

Cada uno de los conceptos descritos en este documento dará lugar a uno o varios capítulos específicos.

Nuestro objetivo no será aprenderlos de memoria.

Nuestro objetivo será comprender cómo encajan entre sí para construir un modelo mental sólido sobre el funcionamiento de la accesibilidad web.

---

> **Las respuestas se olvidan. Los modelos mentales permanecen.**