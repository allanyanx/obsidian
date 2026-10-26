## Etapa 1 — Dart (semanas 1–6, 60 h)

| Semana | Módulos | Contenido                                           | Entregable                                           |
| ------ | ------- | --------------------------------------------------- | ---------------------------------------------------- |
| 1      | 1–2     | Fundamentos y null safety                           | 15 ejercicios cortos en DartPad                      |
| 2      | 3–4     | Funciones y colecciones                             | Procesar una lista de datos con `map`/`where`/`fold` |
| 3      | 5       | POO completa: clases, herencia, mixins, extensiones | Modelar un dominio (p. ej. biblioteca)               |
| 4      | 6–8     | Records, patterns, genéricos, errores               | Refactorizar la semana 3 con `sealed` y `switch`     |
| 5      | 9–10    | Asincronía, streams, isolates, pub                  | Script que consume una API y guarda en archivo       |
| 6      | —       | **Proyecto:** gestor de tareas en consola           | Repositorio con lints sin avisos                     |

## Etapa 2 — Flutter básico (semanas 7–13, 70 h)

|Semana|Módulos|Contenido|Entregable|
|---|---|---|---|
|7|11–12|Entorno, widgets, ciclo de vida|Contador y pantalla de perfil estática|
|8|13|Layout, listas, slivers|Clonar 2 pantallas de apps conocidas|
|9|14–15|Widgets de interfaz, temas, Material 3|Tema claro/oscuro propio|
|10|16–17|Responsivo, gestos, formularios|Formulario de registro con validación|
|11|18|Navegación y `go_router`|App de 4 pantallas con pestañas y deep link|
|12–13|—|**Proyecto:** app de notas|CRUD en memoria, búsqueda, tema y navegación|

## Etapa 3 — Intermedio (semanas 14–21, 80 h)

|Semana|Módulos|Contenido|Entregable|
|---|---|---|---|
|14|19 (a)|`setState`, `InheritedWidget`, notifiers, Provider|Migrar las notas a Provider|
|15|19 (b)|Riverpod **o** BLoC (elige uno y profundiza)|Migrar las notas a la opción elegida|
|16|20|`FutureBuilder`, estados de carga, paginación|Lista infinita con pull to refresh|
|17|21|HTTP, JSON, `freezed`, autenticación|Capa de red con interceptores y manejo de errores|
|18|22|Persistencia: preferencias, SQLite/Drift, caché|Notas persistidas en base de datos|
|19|23|Arquitectura en capas, repositorios, DI, flavors|Reestructurar un proyecto por features|
|20–21|—|**Proyecto:** cliente de API pública|Login, caché offline y arquitectura limpia|

## Etapa 4 — Avanzado (semanas 22–29, 80 h)

|Semana|Módulos|Contenido|Entregable|
|---|---|---|---|
|22|24|Animaciones implícitas, explícitas, `Hero`, `CustomPainter`|3 microinteracciones y un gráfico dibujado a mano|
|23|25|Permisos, cámara, ubicación, notificaciones|Demo con foto geolocalizada y notificación local|
|24|26|Platform Channels, Pigeon, configuración nativa|Leer el nivel de batería con canal propio|
|25|27|Firebase o Supabase: auth, base de datos, push|Login y datos en tiempo real|
|26|28|Internacionalización y accesibilidad|App en 2 idiomas, auditada con lector de pantalla|
|27|29|Pruebas unitarias, de widgets, golden e integración|Cobertura del 70 % en la lógica de un proyecto anterior|
|28–29|—|**Proyecto:** app con mapas, push y animaciones|Con pruebas y backend real|

## Etapa 5 — Profesional (semanas 30–32, 30 h)

|Semana|Módulos|Contenido|Entregable|
|---|---|---|---|
|30|30–31|DevTools, optimización, seguridad, ofuscación|Informe de rendimiento antes/después|
|31|32 (a)|Firma, flavors, CI/CD|Pipeline que compila y ejecuta pruebas en cada push|
|32|32 (b)|Publicación en tiendas|App en prueba interna de Google Play o TestFlight|

## Cómo repartir cada semana

- **30 % teoría** (unas 3 h): documentación oficial y un recurso de apoyo.
- **60 % práctica** (unas 6 h): escribir código sin copiar; el entregable es lo que cuenta.
- **10 % repaso** (1 h): rehacer de memoria algo de la semana anterior.

## Puntos de control

- **Semana 6:** si aún dudas con null safety o `async`/`await`, repite las semanas 2 y 5 antes de pasar a Flutter.
- **Semana 13:** deberías poder construir cualquier pantalla estática viendo solo un diseño.
- **Semana 21:** deberías poder explicar por dónde viaja un dato desde la API hasta el widget.
- **Semana 29:** nivel suficiente para aportar en un equipo como perfil junior.

Publicar en iOS requiere una Mac y la cuenta de desarrollador de Apple (99 USD al año); en Android basta el pago único de 25 USD de Google Play.