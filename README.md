# TFG - Agentes de IA en CyberBattleSim

## Título provisional

**Diseño y evaluación de agentes inteligentes para simulaciones de ciberseguridad mediante CyberBattleSim**

## Descripción

Este Trabajo de Fin de Grado estudia el uso de agentes de inteligencia artificial en entornos simulados de ciberseguridad mediante CyberBattleSim.

El objetivo es analizar cómo distintos tipos de agentes toman decisiones dentro de un entorno de ataque simulado, comparando su comportamiento mediante métricas reproducibles.

El proyecto parte de los agentes baseline incluidos en CyberBattleSim y plantea posteriormente la integración de agentes basados en modelos de lenguaje.

## Objetivos

- Comprender el funcionamiento interno de CyberBattleSim.
- Analizar las observaciones, acciones y recompensas disponibles.
- Estudiar los agentes baseline existentes.
- Diseñar e integrar nuevos agentes de IA.
- Evaluar y comparar distintos enfoques bajo las mismas condiciones.
- Analizar las ventajas, limitaciones y costes de cada enfoque.

## Estado actual

Actualmente se ha:

- Instalado CyberBattleSim correctamente.
- Configurado un entorno virtual con Python 3.10.
- Verificado el uso de CUDA mediante PyTorch.
- Ejecutado correctamente el baseline incluido en CyberBattleSim.
- Probado los agentes DQL y Random Search.
- Preparado la estructura inicial del repositorio.
- Creado documentación de estado y decisiones técnicas.

El proyecto se encuentra actualmente en la fase de comprensión del entorno y análisis de la interfaz entre agentes y CyberBattleSim.

Para más detalle:

- `docs/estado.md`
- `docs/decisiones.md`

## Estructura del repositorio

```markdown
.
├── docs/        # Documentación técnica y decisiones del proyecto
├── notebooks/   # Exploración, visualización y análisis
├── scripts/     # Scripts propios del TFG
├── results/     # Resultados, gráficas y datos generados
└── README.md