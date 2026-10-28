# 03 · Dónde implementar los cambios

| Capa | Qué cambiar | Dónde buscar |
|---|---|---|
| Interfaz | Estilo del botón compuesto (naranja + ícono), banner "Ficha abierta", bloqueo de otros compuestos, botones "Cerrar" / "Cancelar" | Actividad de registro (`net.osmtracker.activity`) y listeners de botones |
| Lógica | Mantener el id de la ficha abierta; decidir si crear waypoint o agregar atributo | Mismo flujo que hoy crea el waypoint al tocar un botón |
| Datos | Nueva tabla/relación de atributos por waypoint; marca de estado de la ficha | Esquema y ContentProvider (`net.osmtracker.db`) |
| Exportación | Escribir atributos en `<extensions>` dentro de cada `<wpt>` | Código de exportación GPX (`net.osmtracker.gpx`) |
| Layouts | Marcar qué botones son compuestos (y su lista de atributos) y cuáles simples, sin romper layouts actuales | XML de layouts de botones |
| Pruebas | Pruebas unitarias del agrupamiento y de la exportación | `./gradlew test` |
