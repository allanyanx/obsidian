Mi parte se basa en aportar a los archivos que detectan las horas faltantes.
* **CalcularHorasFaltantesHandler.cs**: es el archivo que tiene el cálculo puro sin base de datos.
* **ConsultaHorasFaltantes.cs**: Esta clase es la que se encarga de consultar los datos en la base de datos, evalúa las quincenas y agrega el último aviso manual a cada empleado, también tiene una función para consultar cuando una notificación fue enviada previamente y evitar registros duplicados.
* **DetectarHorasFaltantesHandler.cs**: Se encarga de escuchar dos eventos el del flujo 1 que es automático y el flujo 2 manual cuando un líder o administrador envia manualmente la notificación por medio de la interfaz, es el que publica HorasFaltantesDetectadas

![[Pasted image 20261014095615.png]]