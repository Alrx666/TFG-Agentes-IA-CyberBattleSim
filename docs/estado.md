# Estado actual del TFG

## Título provisional

**Diseño y evaluación de agentes inteligentes para simulaciones de ciberseguridad mediante CyberBattleSim**

## Estado general

El proyecto se encuentra en una fase inicial de preparación, comprensión del entorno y definición de la arquitectura de trabajo.

CyberBattleSim ya está instalado y funcionando correctamente en el equipo local.

## Entorno técnico

- Sistema principal: Linux / BlackArch.
- CyberBattleSim instalado en un repositorio separado.
- Python 3.10 configurado mediante entorno virtual.
- Entorno virtual creado en `.venv`.
- Dependencias de CyberBattleSim instaladas correctamente.
- Kernel de Jupyter `cybersim` creado.
- PyTorch detecta CUDA correctamente.
- JupyterLab disponible.
- Matplotlib instalado.
- Plotly instalado.

## Pruebas realizadas

Se ha ejecutado correctamente el baseline incluido en CyberBattleSim.

Agentes probados:

- DQL.
- Random Search.

Parámetros de prueba utilizados:

- 5 episodios de entrenamiento para DQL.
- 3 episodios de evaluación para Random Search.
- 100 iteraciones máximas por episodio.
- `chain_size = 4`.
- `ownership_goal = 0.2`.

La simulación terminó correctamente y se generaron resultados de recompensa y visualizaciones del entorno.

## Resultados observados

Recompensas obtenidas por DQL:

- 154
- 154
- 154
- 154
- 145

Recompensas obtenidas por Random Search:

- 145
- 278
- 154

Estos resultados solo se consideran una comprobación funcional. La muestra es demasiado pequeña para extraer conclusiones sobre el rendimiento de los agentes.

## Warnings observados

Durante la ejecución aparecieron varios warnings relacionados con:

- Uso de atributos de Gymnasium marcados como deprecated.
- Diferencias de tipos NumPy en observaciones.
- Creación poco eficiente de tensores desde listas de arrays.
- Backend no interactivo de Matplotlib.
- Ausencia de `render_fps` en el entorno.

Ninguno de estos avisos impidió la ejecución del baseline.

## Comprensión actual del entorno

Se ha observado que CyberBattleSim representa:

- Nodos de red.
- Máquinas comprometidas (`owned`).
- Máquinas descubiertas (`discovered`).
- Propiedades de los nodos.
- Acciones locales.
- Acciones remotas.
- Conexiones y movimiento lateral.
- Recompensas asociadas a las acciones.

## Próximo objetivo técnico

Antes de implementar agentes nuevos, se debe comprender con precisión:

1. Qué entorno se está utilizando.
2. Qué observaciones recibe el agente.
3. Qué acciones puede ejecutar.
4. Cómo se valida una acción.
5. Cómo se calcula la recompensa.
6. Cómo funciona el agente DQL incluido.
7. Dónde se puede integrar un agente basado en LLM.

## Próximo objetivo de organización

Mantener el repositorio propio separado del repositorio original de CyberBattleSim.

La documentación, scripts, notebooks y resultados del TFG deberán mantenerse en:

`TFG-Agentes-IA-CyberBattleSim/`
