# Prácticas de Fundamentos de Python · Universidad de las Hespérides

## Instalación breve

Necesitas Git y Python 3.12. Clona el repositorio y crea un entorno aislado:

```sh
git clone https://github.com/aprendesc/practicas_fundamentos_python_hesperides.git
cd practicas_fundamentos_python_hesperides
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m ipykernel install --prefix .venv --name practicas_fundamentos_python_hesperides --display-name "Python (Fundamentos de Python)"
python -m jupyter lab
```

En Windows, activa el entorno con `.venv\Scripts\activate` en lugar de `source`.
En JupyterLab selecciona el kernel **Python (Fundamentos de Python)** del entorno y abre un notebook de `practicas/`.
Si ya tienes otro entorno, puedes usar un nombre de carpeta diferente en el primer comando y activarlo.

## Prácticas

Las prácticas están agrupadas por capítulos en `practicas/capitulo_*/`. La numeración de práctica mantiene el recorrido recomendado de la lista siguiente, también cuando un ejercicio integra contenidos de varios capítulos.

Completa el código iniciado. Los objetivos y pequeñas indicaciones están en cada enunciado; las referencias teóricas son opcionales. Ejecuta en orden desde la carpeta del notebook. No se incluyen comprobaciones automáticas: verifica los resultados de tu código. Una celda posterior puede fallar mientras un hueco siga sin completar.

- [01 · Fundamentos de Python: valores, colecciones y control condicional](practicas/capitulo_00_base_python/practica_01_fundamentos_de_python_valores_colecciones_y_control_condicional.ipynb)
- [02 · Fundamentos de Python: iteración, funciones y archivos](practicas/capitulo_00_base_python/practica_02_fundamentos_de_python_iteracion_funciones_y_archivos.ipynb)
- [03 · Implementación de una máquina de Turing](practicas/capitulo_02/practica_03_implementacion_de_una_maquina_de_turing.ipynb)
- [04 · Circuitos lógicos, sumadores y ALU](practicas/capitulo_02/practica_04_circuitos_logicos_sumadores_y_alu.ipynb)
- [05 · Simulación de un computador de programa almacenado](practicas/capitulo_03/practica_05_simulacion_de_un_computador_de_programa_almacenado.ipynb)
- [06 · Representación binaria, codificación y detección de errores](practicas/capitulo_01/practica_06_representacion_binaria_codificacion_y_deteccion_de_errores.ipynb)
- [07 · Serialización y comunicación mediante sockets](practicas/capitulo_04/practica_07_serializacion_y_comunicacion_mediante_sockets.ipynb)
- [08 · Concurrencia, idempotencia y replicación](practicas/capitulo_05/practica_08_concurrencia_idempotencia_y_replicacion.ipynb)

Los datos de práctica están incluidos en el repositorio. El archivo `resultado_local.txt`, cuando se utiliza, se crea junto al notebook; puedes borrarlo para repetir.

## Exámenes

`examenes/` contiene únicamente `.gitkeep` para conservar la carpeta en Git. No hay exámenes publicados. Aquí aparecerán los exámenes práctico y teórico cuando se pongan a disposición.
