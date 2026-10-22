# Banc de proves Henry — normas del proyecto

## Descripción

Calculadora de código de colores de resistencias de 4 y 5 bandas, según la
norma IEC 60062. Debe permitir:

- Convertir de colores a valor (ohmios, incluyendo la tolerancia).
- Convertir de valor a colores.

## Tecnología

- Python 3.14, en Windows.
- El ejecutable final se genera con PyInstaller.
- Pruebas automáticas con pytest.

## Idioma

- Nombres de variables y funciones: en inglés.
- Comentarios, documentación y mensajes de commit: en castellano.
- Los comentarios deben ser comprensibles para alguien que sabe de
  electrónica pero no es programador profesional. Evitar jerga de
  programación innecesaria; preferir explicar el "por qué" en términos de
  electrónica (bandas, tolerancia, coeficiente de temperatura, etc.).

## Flujo de trabajo

- Nunca trabajar directamente en `main`.
- Cada tarea se desarrolla en una rama nueva.
- Commits pequeños y descriptivos.
- Al terminar una tarea, abrir un pull request hacia `main`.
- Nunca fusionar pull requests: esa acción la realiza siempre el usuario.

## Archivos

- No borrar archivos. Si parece necesario eliminar algo, proponerlo al
  usuario y que sea él quien lo decida.

## Cambios grandes

- Antes de acometer cambios grandes, presentar un plan y esperar la
  aprobación del usuario.
