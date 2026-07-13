## Commit messages

Este proyecto sigue la filosofía de **Conventional Commits**, adaptada a un proyecto de documentación técnica.

Todos los mensajes de commit deben seguir el siguiente formato:

```text
<type>: <short description>
```

La descripción debe:

- Estar escrita en **inglés**.
- Utilizar el **modo imperativo**.
- Ser breve y descriptiva.
- Empezar en minúscula.
- No terminar con punto.

### Tipos de commit

| Tipo | Uso |
|------|-----|
| `feat` | Nueva funcionalidad del proyecto. |
| `docs` | Cambios en el handbook o documentación. |
| `research` | Nuevas investigaciones, experimentos o debates técnicos. |
| `academy` | Material de estudio, cuestionarios y simulacros. |
| `fix` | Corrección de errores o información incorrecta. |
| `refactor` | Reorganización del contenido sin modificar su significado. |
| `style` | Cambios de formato, ortografía o estilo. |
| `test` | Pruebas o validaciones del proyecto. |
| `chore` | Tareas de mantenimiento. |

### Ejemplos

```text
docs: add project manifesto

docs: define learning methodology

research: investigate anchors without href

academy: add first WAS practice quiz

fix: correct accessible name example

refactor: reorganize handbook structure

style: improve markdown formatting

chore: add github templates
```

### Commits pequeños y atómicos

Cada commit debe representar un único cambio lógico.

Es preferible realizar varios commits pequeños que uno muy grande.

### Buenas prácticas

- Un commit debe poder entenderse únicamente leyendo su mensaje.
- Evita mezclar cambios de distinta naturaleza en un mismo commit.
- Mantén el historial limpio y fácil de seguir.
- Si el cambio requiere más contexto, añade una descripción en el cuerpo del commit.