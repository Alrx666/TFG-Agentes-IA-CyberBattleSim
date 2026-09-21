# TFG - Agentes de IA en CyberBattleSim

## Título provisional

**Diseño y evaluación de agentes inteligentes para simulaciones de ciberseguridad mediante CyberBattleSim**

## Objetivo

El objetivo de este Trabajo de Fin de Grado es estudiar, integrar y evaluar agentes de inteligencia artificial dentro de entornos simulados de ciberseguridad utilizando CyberBattleSim.

La idea principal es analizar cómo distintos tipos de agentes toman decisiones dentro de un entorno de ataque simulado y comparar su comportamiento mediante métricas reproducibles.

## Punto de partida

Actualmente se ha:

- Instalado CyberBattleSim correctamente.
- Configurado su entorno virtual con Python 3.10.
- Verificado que PyTorch detecta CUDA.
- Ejecutado correctamente el baseline incluido en CyberBattleSim.
- Probado los agentes:
  - DQL
  - Random Search

## Línea de trabajo prevista

El proyecto se desarrollará de forma incremental:

1. Comprender el funcionamiento de CyberBattleSim.
2. Analizar sus entornos, acciones, observaciones y sistema de recompensas.
3. Estudiar los agentes baseline disponibles.
4. Identificar el punto de integración para nuevos agentes.
5. Implementar uno o varios agentes basados en IA.
6. Diseñar experimentos reproducibles.
7. Comparar los agentes mediante métricas comunes.
8. Analizar los resultados obtenidos.

## Estructura del repositorio

```text
.
├── docs/        # Documentación y memoria técnica
├── notebooks/   # Experimentos y análisis interactivos
├── scripts/     # Scripts propios del proyecto
├── results/     # Resultados, gráficas y datos
└── README.md