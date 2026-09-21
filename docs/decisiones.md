# Decisiones del proyecto

Este archivo recoge decisiones técnicas y de organización relevantes para el TFG.

## 1. Mantener CyberBattleSim separado

### Decisión

El repositorio oficial de CyberBattleSim se mantiene separado del repositorio propio del TFG.

### Motivo

Esto permite:

- Evitar modificar directamente el código original de Microsoft.
- Mantener claro qué código pertenece al proyecto propio.
- Facilitar actualizaciones futuras de CyberBattleSim.
- Mejorar la trazabilidad de los cambios realizados en el TFG.

## 2. Crear un repositorio propio para el TFG

### Decisión

Se utiliza un repositorio independiente llamado:

`TFG-Agentes-IA-CyberBattleSim`

### Motivo

El repositorio propio servirá para almacenar:

- Documentación.
- Notebooks.
- Scripts.
- Experimentos.
- Resultados.
- Decisiones de diseño.

## 3. Usar documentación viva

### Decisión

Se utilizará la carpeta `docs/` como memoria técnica del proyecto.

### Motivo

Esto facilita:

- Mantener contexto entre sesiones.
- Documentar decisiones.
- Registrar el progreso.
- Ayudar a herramientas como Codex a comprender el estado del proyecto.
- Reutilizar material posteriormente en la memoria final del TFG.

## 4. Utilizar Jupyter para exploración

### Decisión

Los notebooks se utilizarán para:

- Comprender CyberBattleSim.
- Explorar datos y resultados.
- Visualizar recompensas.
- Analizar comportamiento de agentes.

### Motivo

Jupyter facilita el análisis interactivo y la visualización.

La lógica reutilizable no debe quedarse únicamente en notebooks y deberá moverse a scripts o módulos cuando sea necesario.

## 5. No actualizar dependencias sin necesidad

### Decisión

No se actualizarán automáticamente paquetes como Pyright, npm u otras dependencias si la instalación actual funciona correctamente.

### Motivo

Actualizar dependencias sin necesidad puede introducir incompatibilidades y reducir la reproducibilidad del entorno.

## 6. Usar los baselines como referencia

### Decisión

Los agentes incluidos en CyberBattleSim, como DQL y Random Search, se utilizarán como puntos de referencia.

### Motivo

Permiten establecer una base de comparación antes de implementar agentes nuevos.

## 7. No extraer conclusiones de las primeras ejecuciones

### Decisión

Las primeras ejecuciones se consideran únicamente pruebas funcionales.

### Motivo

Un número pequeño de episodios no permite comparar agentes de forma fiable.

Los experimentos finales deberán usar:

- Más episodios.
- Semillas controladas.
- Condiciones comparables.
- Métricas consistentes.
- Varias repeticiones cuando sea necesario.

## 8. Priorizar reproducibilidad

### Decisión

Todo experimento importante deberá registrar, cuando sea posible:

- Entorno.
- Agente.
- Parámetros.
- Semilla.
- Episodios.
- Iteraciones.
- Métricas.
- Tiempo de ejecución.
- Modelo utilizado.
- Coste o tokens si interviene un LLM.

### Motivo

La reproducibilidad será un criterio central del proyecto y facilitará la comparación entre agentes.
