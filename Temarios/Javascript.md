# Temario completo de JavaScript

## 1. Fundamentos

- Qué es JavaScript, ECMAScript y sus versiones
- Dónde se ejecuta: navegador, Node.js, consola
- Sintaxis básica, comentarios, `"use strict"`
- Variables: `var`, `let`, `const`; ámbito y hoisting
- Tipos de datos: primitivos (`string`, `number`, `bigint`, `boolean`, `null`, `undefined`, `symbol`) y objetos
- Conversión de tipos y coerción; `==` vs `===`
- Operadores: aritméticos, lógicos, comparación, ternario, `??`, `?.`

## 2. Control de flujo

- `if / else`, `switch`
- Bucles: `for`, `while`, `do...while`, `for...of`, `for...in`
- `break`, `continue`, etiquetas
- Manejo de errores: `try / catch / finally`, `throw`, errores personalizados

## 3. Funciones

- Declaración, expresión y funciones flecha
- Parámetros por defecto, rest y spread
- Ámbito léxico y closures
- `this`, `call`, `apply`, `bind`
- Funciones de orden superior, callbacks, recursión
- IIFE, funciones puras, currying y composición

## 4. Estructuras de datos

- Strings: métodos, template literals, expresiones regulares
- Arrays: `map`, `filter`, `reduce`, `find`, `some`, `every`, `sort`, `flat`, etc.
- Objetos: propiedades, métodos, desestructuración, `Object.keys/values/entries`
- `Map`, `Set`, `WeakMap`, `WeakSet`
- JSON: `parse` y `stringify`
- Fechas (`Date`, `Intl`) y `Math`
- Copia superficial vs profunda, inmutabilidad

## 5. Programación orientada a objetos

- Prototipos y cadena de prototipos
- Clases: constructor, métodos, `static`, campos privados (`#`)
- Herencia: `extends`, `super`
- Getters y setters
- Encapsulamiento, polimorfismo, composición vs herencia

## 6. Asincronía

- Event loop, call stack, microtareas y macrotareas
- `setTimeout`, `setInterval`
- Callbacks y "callback hell"
- Promesas: `then`, `catch`, `finally`, `Promise.all / allSettled / race / any`
- `async / await` y manejo de errores
- `fetch`, consumo de APIs REST, `AbortController`

## 7. JavaScript en el navegador

- DOM: selección, creación, modificación y eliminación de nodos
- Eventos: listeners, propagación (bubbling/capturing), delegación
- Formularios y validación
- BOM: `window`, `location`, `history`, `navigator`
- Almacenamiento: `localStorage`, `sessionStorage`, cookies, IndexedDB
- APIs web: Geolocation, Canvas, Web Workers, WebSockets, Intersection Observer, Service Workers

## 8. JavaScript moderno (ES6+)

- Módulos: `import` / `export`, imports dinámicos
- Desestructuración, spread/rest
- Iteradores y generadores
- `Symbol`, `Proxy`, `Reflect`
- Novedades recientes de cada versión de ECMAScript

## 9. Herramientas y ecosistema

- Node.js y npm / pnpm / yarn
- Bundlers: Vite, Webpack, esbuild
- Babel, ESLint, Prettier
- Git y control de versiones
- Depuración con DevTools

## 10. Testing

- Tipos: unitarias, integración, end-to-end
- Jest / Vitest
- Testing Library, Playwright / Cypress
- Mocks, cobertura, TDD

## 11. Temas avanzados

- Patrones de diseño (módulo, observer, factory, singleton…)
- Programación funcional
- Gestión de memoria y garbage collector
- Rendimiento: debounce, throttle, lazy loading, memoización
- Seguridad: XSS, CSRF, CORS, sanitización
- Estructuras de datos y algoritmos en JS

## 12. Siguientes pasos

- **TypeScript**: tipos, interfaces, genéricos
- **Frontend**: React, Vue, Angular o Svelte
- **Backend**: Node.js con Express / NestJS, bases de datos, autenticación
- **Móvil**: React Native
- **Full-stack**: Next.js, Nuxt

---

**Orden recomendado:** secciones 1 → 4 (base), luego 7 con proyectos pequeños, después 5, 6 y 8, y finalmente 9 → 12.

