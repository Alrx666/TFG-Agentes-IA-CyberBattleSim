# Primera prueba funcional de CyberBattleSim

## Objetivo

Comprobar que CyberBattleSim está correctamente instalado y que los agentes baseline pueden ejecutarse sin errores críticos.

## Comando utilizado

python -m cyberbattle.agents.baseline.run \
  --training_episode_count 5 \
  --eval_episode_count 3 \
  --iteration_count 100 \
  --rewardplot_width 80 \
  --chain_size 4 \
  --ownership_goal 0.2

## Resultado

La simulación terminó correctamente.

Se ejecutaron:

- DQL
- Random Search

Resultados observados:

### DQL

- 154
- 154
- 154
- 154
- 145

### Random Search

- 145
- 278
- 154

## Observaciones

Durante la ejecución aparecieron warnings de Gymnasium, PyTorch y Matplotlib, pero ninguno impidió la simulación.

PyTorch detectó CUDA correctamente.

También se generaron visualizaciones del entorno y del reward acumulado.

## Conclusión

La instalación de CyberBattleSim funciona correctamente.

Esta prueba no se considera un experimento válido para comparar el rendimiento entre agentes, ya que el número de episodios es demasiado pequeño.

Su objetivo fue únicamente validar el entorno.

## Evidencias

Salida completa de terminal:

`primer_baseline_terminal.txt`

Capturas:

- Evolución del reward acumulado.
- Estado de la red simulada al finalizar la ejecución.