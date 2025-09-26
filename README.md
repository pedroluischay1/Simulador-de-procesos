📌 Simulador de Planificación de Procesos
Este proyecto implementa un simulador gráfico de algoritmos de planificación de procesos en Java, utilizando Swing para la interfaz gráfica.

Permite crear procesos con parámetros personalizados (nombre, tiempo de CPU, instante de llegada y quantum en caso de Round Robin) y simular su ejecución con distintos algoritmos de planificación.

✨ Características

Interfaz gráfica amigable desarrollada con Java Swing.

Posibilidad de agregar procesos manualmente con:
-Nombre
-Tiempo de CPU (unidades)
-Instante de llegada (unidades)
-Quantum (solo en Round Robin)

Selección de algoritmo de planificación:
🔹 FCFS (First Come, First Served)
🔹 SJF (Shortest Job First)
🔹 SRTF (Shortest Remaining Time First)
🔹 Round Robin

Visualización en tiempo real de:
-Cola de procesos listos
-Historial de procesos finalizados
-Simulación de tiempo configurable (en este caso 1 unidad = 5 segundos).
-Posibilidad de limpiar historial y cola de procesos.

🖼️ Interfaz

La aplicación cuenta con:
-Panel de entrada: para ingresar datos de nuevos procesos.
-Tablas: una para la cola de procesos y otra para el historial de finalización.
-Panel de control: botones para iniciar simulación y limpiar datos.

⚙️ Requisitos

-Java JDK 8 o superior
-Cualquier IDE compatible con Java (IntelliJ IDEA, Eclipse, NetBeans) o compilación por consola.

🚀 Instalación y ejecución

-Clonar este repositorio o copiar el código fuente.
-Compilar el archivo SimuladorPlanificacion.java:
-javac SimuladorPlanificacion.java


Ejecutar la aplicación:

-java SimuladorPlanificacion
-📊 Algoritmos soportados

1. FCFS (First Come, First Served)
-Procesos se ejecutan en el orden en que llegan, sin interrupciones.

2. SJF (Shortest Job First)
-Se selecciona siempre el proceso con menor tiempo de CPU total.

3. SRTF (Shortest Remaining Time First)
-Versión expropiativa del SJF. Se ejecuta el proceso con menor tiempo restante.

4. Round Robin (RR)
-Cada proceso recibe un quantum definido. Si no finaliza en ese tiempo, regresa al final de la cola.

📝 Uso básico

-Ingresar datos de un proceso en el panel de entrada.
-Seleccionar el algoritmo de planificación.
-Hacer clic en Agregar Proceso.
-Repetir para tantos procesos como se desee.
-Pulsar Iniciar Simulación para observar la ejecución.
-Usar Limpiar Historial y Cola para reiniciar la simulación.

📌 Notas

-Cada unidad de tiempo en la simulación equivale a 5 segundos en la vida real.
-El quantum solo se habilita cuando se selecciona el algoritmo Round Robin.
-Los resultados finales se muestran en un cuadro de diálogo al terminar la simulación.
