# Temario completo de C#: de lo general a lo específico

Estructura: **8 niveles → módulos → temas**. Cada nivel cierra con un proyecto práctico. Las versiones de referencia son **C# 14 / .NET 10 (LTS)**.

---

## NIVEL 0 — Fundamentos previos (contexto)

### 0.1 Qué es programar

- Algoritmos, pseudocódigo y diagramas de flujo
- Lenguajes compilados frente a interpretados
- Tipado estático frente a dinámico

### 0.2 El ecosistema .NET

- Historia: .NET Framework → .NET Core → .NET moderno
- CLR (Common Language Runtime), IL (Intermediate Language) y JIT
- BCL (Base Class Library)
- SDK frente a Runtime; versiones LTS y STS
- NuGet: gestor de paquetes

### 0.3 Entorno de trabajo

- Instalar el .NET SDK
- IDEs: Visual Studio, VS Code con C# Dev Kit, JetBrains Rider
- CLI: `dotnet new`, `dotnet build`, `dotnet run`, `dotnet add package`
- Estructura de un proyecto: `.csproj`, `.sln`/`.slnx`, `bin/` y `obj/`
- Git básico

**🛠 Proyecto:** "Hola Mundo" creado y ejecutado desde la CLI y desde el IDE.

---

## NIVEL 1 — Sintaxis básica

### 1.1 Estructura de un programa

- Top-level statements frente a `Main`
- Namespaces (incluidos los _file-scoped_) y `using`
- Comentarios y documentación XML (`///`)

### 1.2 Variables y tipos

- Tipos primitivos: `int`, `long`, `double`, `decimal`, `bool`, `char`, `string`
- `var` e inferencia de tipos
- Constantes (`const`) y `readonly`
- Literales, separadores (`1_000_000`), hexadecimal y binario
- Conversiones: implícitas, explícitas (cast), `Convert`, `Parse` y `TryParse`

### 1.3 Operadores

- Aritméticos, relacionales y lógicos
- Asignación compuesta, incremento y decremento
- Operadores de null: `?.`, `??`, `??=`
- Operador ternario
- Precedencia

### 1.4 Entrada y salida

- `Console.WriteLine` y `Console.ReadLine`
- Interpolación de strings (`$""`), strings verbatim (`@""`) y raw strings (`"""`)
- Formatos numéricos y de fecha

### 1.5 Control de flujo

- `if` / `else`
- `switch` clásico y _switch expressions_
- Bucles: `for`, `while`, `do-while`, `foreach`
- `break`, `continue` y `return`

### 1.6 Métodos

- Declaración, parámetros y retorno
- Parámetros opcionales y nombrados
- `ref`, `out`, `in` y `params`
- Sobrecarga
- Funciones locales
- Recursión

### 1.7 Arrays y strings

- Arrays unidimensionales, multidimensionales y jagged
- Métodos de `string`: `Split`, `Substring`, `Replace`, `Trim`…
- Inmutabilidad de los strings y `StringBuilder`
- _Collection expressions_ (`[1, 2, 3]`)

**🛠 Proyecto:** calculadora de consola, juego de adivinar el número o conversor de unidades.

---

## NIVEL 2 — Programación orientada a objetos (POO)

### 2.1 Clases y objetos

- Campos, propiedades (auto-properties, `init`, `required`, palabra clave `field`)
- Constructores, constructores primarios y encadenamiento con `this(...)`
- Modificadores de acceso: `public`, `private`, `protected`, `internal`, `file`…
- Miembros `static` y clases estáticas
- Inicializadores de objetos

### 2.2 Los cuatro pilares

- **Encapsulamiento**
- **Herencia**: `base`, `sealed`
- **Polimorfismo**: `virtual`, `override`, `new`
- **Abstracción**: clases `abstract`

### 2.3 Interfaces

- Definición e implementación
- Implementación explícita
- Métodos por defecto en interfaces
- Miembros estáticos abstractos (_generic math_)

### 2.4 Tipos de valor frente a tipos de referencia

- `struct` frente a `class`
- Stack frente a heap (modelo mental)
- Boxing y unboxing
- `record`, `record struct`, igualdad por valor y expresiones `with`
- `enum` y flags
- Tuplas y deconstrucción

### 2.5 La clase `object`

- `ToString`, `Equals` y `GetHashCode`
- Sobrecarga de operadores
- Indexadores
- Métodos de extensión y _extension members_ (C# 14)

### 2.6 Principios de diseño

- SOLID
- DRY, KISS y YAGNI
- Composición frente a herencia

**🛠 Proyecto:** sistema de gestión de biblioteca o de cuentas bancarias con jerarquía de clases.

---

## NIVEL 3 — Núcleo intermedio del lenguaje

### 3.1 Manejo de errores

- `try` / `catch` / `finally`
- Jerarquía de excepciones
- Excepciones personalizadas
- `throw` frente a `throw ex`, y filtros `when`
- Buenas prácticas: cuándo **no** usar excepciones

### 3.2 Nulabilidad

- Nullable value types (`int?`)
- Nullable reference types (NRT) y sus advertencias
- Operador `!` (null-forgiving)

### 3.3 Genéricos

- Clases y métodos genéricos
- Restricciones (`where T : ...`)
- Covarianza y contravarianza (`in` / `out`)

### 3.4 Colecciones

- `List<T>`, `Dictionary<TKey,TValue>`, `HashSet<T>`, `Queue<T>`, `Stack<T>`, `LinkedList<T>`
- `IEnumerable<T>`, `ICollection<T>`, `IList<T>`, `IReadOnly*`
- Colecciones inmutables y _frozen collections_
- Complejidad algorítmica (Big O) de cada una

### 3.5 Delegados y eventos

- `delegate`, `Action`, `Func`, `Predicate`
- Expresiones lambda
- Eventos y el patrón `EventHandler`
- Closures

### 3.6 LINQ

- Sintaxis de métodos frente a sintaxis de consulta
- `Where`, `Select`, `OrderBy`, `GroupBy`, `Join`, `Aggregate`…
- Ejecución diferida frente a inmediata
- `IEnumerable` frente a `IQueryable`

### 3.7 Iteradores

- `yield return`
- Implementar `IEnumerable` a mano

### 3.8 Pattern matching

- Patrones de tipo, constante, relacional y lógico (`and`, `or`, `not`)
- Patrones de propiedad, posicionales y de lista

**🛠 Proyecto:** gestor de inventario con LINQ, filtros, ordenaciones y persistencia en fichero.

---

## NIVEL 4 — Programación avanzada

### 4.1 Asincronía

- Hilos frente a tareas; qué es realmente `async`
- `Task`, `Task<T>` y `ValueTask`
- `async` / `await` y su máquina de estados
- `CancellationToken`
- `Task.WhenAll` y `Task.WhenAny`
- `IAsyncEnumerable` y `await foreach`
- Errores típicos: `async void`, `.Result` y deadlocks, `ConfigureAwait`

### 4.2 Concurrencia y paralelismo

- `Thread` y `ThreadPool`
- `Parallel.For` / `ForEach` y PLINQ
- Sincronización: `lock`, `Lock` (.NET 9+), `SemaphoreSlim`, `Interlocked`
- Colecciones concurrentes
- `Channel<T>`

### 4.3 Gestión de memoria

- Garbage Collector: generaciones y LOH
- `IDisposable`, `using` e `IAsyncDisposable`
- Finalizadores
- `WeakReference`

### 4.4 Alto rendimiento

- `Span<T>`, `ReadOnlySpan<T>` y `Memory<T>`
- `stackalloc`
- `ref struct`, `ref return` y `ref locals`
- `ArrayPool<T>`
- Código `unsafe` y punteros (nociones)

### 4.5 Reflexión y metaprogramación

- `Type`, `typeof`, `GetType` y reflexión
- Atributos personalizados
- `dynamic`
- Árboles de expresión
- Source Generators

### 4.6 Ficheros y serialización

- `File`, `Directory`, `Path` y `Stream`
- `System.Text.Json`
- XML
- Serialización con source generation

**🛠 Proyecto:** descargador o procesador concurrente de ficheros con async, cancelación y progreso.

---

## NIVEL 5 — Arquitectura y calidad

### 5.1 Testing

- Tests unitarios con xUnit, NUnit o MSTest
- Patrón Arrange-Act-Assert
- Mocks con Moq o NSubstitute
- Tests de integración
- TDD
- Cobertura de código

### 5.2 Inyección de dependencias

- IoC y DI
- `Microsoft.Extensions.DependencyInjection`
- Lifetimes: Singleton, Scoped y Transient

### 5.3 Configuración y logging

- `IConfiguration`, `appsettings.json` y patrón Options
- `ILogger` y logging estructurado (Serilog)

### 5.4 Patrones de diseño

- **Creacionales:** Factory, Builder, Singleton
- **Estructurales:** Adapter, Decorator, Facade
- **De comportamiento:** Strategy, Observer, Command, Mediator
- Repository y Unit of Work

### 5.5 Arquitecturas

- En capas
- Clean Architecture y Hexagonal
- Vertical Slice
- DDD (nociones)
- CQRS

### 5.6 Herramientas

- Analizadores de Roslyn y `.editorconfig`
- Depuración avanzada: breakpoints condicionales y diagnósticos
- Profiling: dotnet-trace, dotnet-counters
- BenchmarkDotNet

**🛠 Proyecto:** refactorizar el proyecto del nivel 3 a Clean Architecture con DI y tests.

---

## NIVEL 6 — Acceso a datos

### 6.1 Bases de datos

- SQL básico: SELECT, JOIN, índices
- ADO.NET

### 6.2 Entity Framework Core

- DbContext y entidades
- Code First y migraciones
- Relaciones: 1:1, 1:N, N:M
- Consultas, tracking y `AsNoTracking`
- Lazy, eager y explicit loading
- Problema N+1
- Transacciones y concurrencia

### 6.3 Alternativas

- Dapper
- Bases NoSQL: MongoDB, Redis
- Caché: `IMemoryCache`, `HybridCache`

---

## NIVEL 7 — Especialización (elige una o varias ramas)

### 7A. Web y backend: ASP.NET Core

- Pipeline y middleware
- Minimal APIs frente a Controllers
- Routing, model binding y validación
- REST y OpenAPI
- Autenticación y autorización: JWT, OAuth2/OIDC, Identity
- SignalR (tiempo real)
- gRPC
- Rate limiting, CORS y health checks
- Blazor (Server, WebAssembly, Auto)

### 7B. Escritorio

- WPF y MVVM
- WinUI 3
- .NET MAUI (multiplataforma)
- Avalonia

### 7C. Videojuegos

- Unity: MonoBehaviour, ciclo de vida, física, corrutinas
- Godot con C#
- MonoGame

### 7D. Cloud y DevOps

- Docker y contenedores
- .NET Aspire
- Azure: App Service, Functions, Service Bus
- CI/CD con GitHub Actions
- Observabilidad con OpenTelemetry
- Microservicios y mensajería (RabbitMQ, MassTransit)

### 7E. IA y datos

- `Microsoft.Extensions.AI`
- Semantic Kernel
- ML.NET
- Integración con APIs de LLMs

### 7F. Sistemas y rendimiento

- Native AOT
- Interop con código nativo (P/Invoke)
- Trimming
- Herramientas CLI y librerías publicables en NuGet

---

## NIVEL 8 — Maestría

- Internals del CLR: JIT, tiered compilation, type loading
- Compilador Roslyn: escribir analizadores y code fixes
- Lectura de IL y SharpLab
- Modelo de memoria y threading a bajo nivel
- Contribuir a proyectos open source (dotnet/runtime)
- Leer el código fuente de la BCL

**🛠 Proyecto final:** aplicación completa de la rama elegida (API + BD + tests + Docker + CI/CD) desplegada en producción.

---

## Ruta sugerida y tiempos orientativos

|Nivel|Duración aprox. (1–2 h/día)|
|---|---|
|0–1|3–4 semanas|
|2|4 semanas|
|3|4–5 semanas|
|4|5–6 semanas|
|5–6|6–8 semanas|
|7|2–4 meses por rama|
|8|Continuo|

## Recursos recomendados

- **Oficial:** Microsoft Learn (learn.microsoft.com/dotnet/csharp)
- **Libros:** _C# in Depth_ (Jon Skeet), _C# 12 in a Nutshell_ (Albahari), _CLR via C#_ (Richter, para el nivel 8)
- **Práctica:** Exercism (track de C#), Codewars, LeetCode
- **Herramientas:** sharplab.io para ver el IL y el código que genera el compilador

