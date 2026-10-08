### Conexiones de API
- Los ID's no pueden estar en los modelos con el nombre Id por inconsistencia en diferentes lenguajes (case by case).
- No deben haber inconsistencias a nivel modelo para el backend principalmente.
- Evitar inconsistencias en scripts para BD's.
- Usar triggers solo si es estrictamente necesario.
### Diseño de app movil
- Solo debe haber lógica de diseño
- En flutter no se pueden definir variables de entorno, sin embargo, se pueden hacer settings para configurar la dirección del backend al que te desees conectar.