# 01 · Análisis del problema

## Limitación
Cada botón de la pantalla de registro crea un waypoint independiente. Un árbol descrito con género, especie y altura genera tres waypoints sin relación explícita y con coordenadas ligeramente distintas (deriva del GPS).

## Cómo el diseño moldea el mapeo
- "Punto" = evento de captura, no elemento del territorio.
- El atributo es la unidad mínima; el conteo de waypoints no coincide con el conteo de elementos.
- OSM modela un nodo con varios tags.

## Actores
Personas mapeadoras, quienes validan en OSM, coordinación del proyecto comunitario, comunidad/gobierno local, mantenedores de OSMTracker.

![Problema actual vs propuesta](img/01-problema-vs-propuesta.png)
