# Prácticas de Fundamentos de Python · Universidad de las Hespérides

Material de clases síncronas y prácticas de Fundamentos de Python, basado en las notas de Programación I de la Universidad de las Hespérides.

## Clase disponible

[Capítulo 1 · Tecnologías, representación y arquitectura del computador](workshop/clases_sincronas/capitulo_1.ipynb): sesión guiada de 90 minutos con ocho bloques, seis ejercicios, cinco exploradores interactivos y 47 minutos de trabajo del alumnado, incluyendo apertura y cierre. Se estudian señales y márgenes, interpretación de bytes, programa almacenado, localidad, ejecución de Python y precisión numérica.

## Organización

- `workshop/clases_sincronas/`: notebooks de las clases publicados para el alumnado, uno por clase.
- `workshop/tareas/`: notebooks de prácticas para resolver.
- `professor/`: espejo docente local, excluido de Git, con soluciones y guías dentro de los notebooks, además de recursos privados de preparación.

## Entorno

Se utiliza Python 3.12 y uv, con dependencias fijadas en `uv.lock`.

```bash
uv sync --locked
uv run jupyter lab
```

El entorno inicial incluye JupyterLab y soporte para notebooks y widgets. Las dependencias específicas se añadirán cuando el material las necesite.

Ejecuta el notebook en orden desde un kernel limpio. Las celdas pendientes muestran mensajes o espacios de respuesta sin impedir la ejecución del soporte. Los controles de las demos funcionan en el navegador y no requieren servicios externos. Si el visor no permite JavaScript, abre el notebook en JupyterLab y ejecuta sus celdas; confía únicamente en notebooks de procedencia conocida.

La edición local del profesor conserva guion oral, pistas y solucionario dentro del mismo notebook. La versión del alumnado mantiene las mismas celdas públicas, sin el contenido privado. El resto del temario está pendiente de preparar.
