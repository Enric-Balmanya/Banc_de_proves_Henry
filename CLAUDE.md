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

## Equipo de subagentes

El proyecto cuenta con cuatro subagentes definidos en `.claude/agents/`:

- **programador**: implementa y corrige la lógica y la interfaz de la
  calculadora.
- **tester**: escribe y ejecuta pruebas con pytest; no corrige código de la
  aplicación, solo informa de errores.
- **revisor**: solo lectura; revisa código y pruebas buscando errores,
  código poco claro y desviaciones de estas normas (con especial atención
  a la corrección según IEC 60062) y entrega un informe.
- **documentador**: mantiene el README y la documentación de uso, en
  castellano y pensada para un usuario sin conocimientos de programación.

Orden habitual de trabajo: programador → tester → revisor →
documentador, volviendo al programador si el tester o el revisor
detectan algún fallo. Los subagentes no crean ramas ni cambian de rama:
siempre trabajan en la rama que ya ha preparado el agente principal.

## Archivos

- No borrar archivos. Si parece necesario eliminar algo, proponerlo al
  usuario y que sea él quien lo decida.

## Cambios grandes

- Antes de acometer cambios grandes, presentar un plan y esperar la
  aprobación del usuario.
