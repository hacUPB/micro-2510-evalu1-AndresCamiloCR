# CONCEPTOS

## 1. CPU (Central Processing Unit):
La CPU (Unidad Central de Procesamiento) es el componente principal de una computadora, encargado de ejecutar las instrucciones de los programas y procesar los datos. Actúa como el "cerebro" del sistema, ya que realiza operaciones aritméticas, lógicas y de control. La CPU está compuesta por varios subcomponentes, como la ALU (Unidad Aritmético-Lógica), la Unidad de Control y los registros. Su rendimiento se mide en términos de velocidad de reloj (GHz) y la cantidad de instrucciones que puede procesar por segundo.

Funciones principales:

Ejecutar instrucciones de programas.

Realizar cálculos aritméticos y lógicos.

Controlar el flujo de datos entre los diferentes componentes del sistema.

## 2. ALU (Arithmetic Logic Unit)
La ALU (Unidad Aritmético-Lógica) es un componente clave de la CPU que se encarga de realizar operaciones aritméticas (como suma, resta, multiplicación y división) y operaciones lógicas (como AND, OR, NOT y XOR). La ALU trabaja con datos provenientes de los registros y devuelve los resultados a estos mismos registros o a la memoria principal.

Características:

Opera con datos binarios.

Puede manejar operaciones en enteros y, en algunos casos, en números de punto flotante.

Está controlada por señales de la Unidad de Control.

## 3. Registros
Los registros son pequeñas unidades de almacenamiento de alta velocidad ubicadas dentro de la CPU. Se utilizan para almacenar datos temporalmente durante la ejecución de instrucciones. Los registros son esenciales para optimizar el rendimiento, ya que permiten un acceso rápido a los datos en comparación con la memoria principal.

a) Registros de propósito general
Estos registros son utilizados para almacenar datos y resultados intermedios en operaciones generales. Su uso no está restringido a una tarea específica, lo que los hace versátiles.

b) Registros específicos
Program Counter (PC): Almacena la dirección de memoria de la siguiente instrucción que se va a ejecutar. Se incrementa automáticamente después de cada ciclo de instrucción.

Stack Pointer (SP): Apunta a la dirección superior de la pila (stack), que es una estructura de datos utilizada para almacenar temporalmente direcciones de retorno y datos locales durante la ejecución de subrutinas.

## 4. Unidad de control
La Unidad de Control es un componente crítico de la CPU que dirige y coordina las operaciones de los demás componentes. Su función principal es interpretar las instrucciones del programa y generar las señales de control necesarias para ejecutarlas. La Unidad de Control se encarga de gestionar el flujo de datos entre la CPU, la memoria y los dispositivos de entrada/salida.

Funciones principales:

Decodificar las instrucciones del programa.

Generar señales de control para la ALU, los registros y otros componentes.

Coordinar el ciclo de instrucción (fetch, decode, execute).

## 5. Buses de datos y de dirección
Los buses son canales de comunicación que permiten la transferencia de datos y señales entre los componentes de la computadora.

Bus de datos: Transfiere datos entre la CPU, la memoria y los dispositivos de entrada/salida. Su ancho (en bits) determina la cantidad de datos que puede transferir simultáneamente.

Bus de dirección: Especifica las direcciones de memoria que la CPU necesita leer o escribir. Su ancho determina la cantidad máxima de memoria que puede direccionar.

Ejemplo: Un bus de datos de 64 bits puede transferir 64 bits de datos en paralelo, mientras que un bus de dirección de 32 bits puede direccionar hasta 4 GB de memoria.

## 6. Memoria RAM y memoria ROM
RAM (Random Access Memory): Es una memoria volátil que almacena datos y programas en ejecución. La RAM permite lecturas y escrituras rápidas, pero pierde su contenido cuando se apaga la computadora. Es esencial para el rendimiento del sistema, ya que determina la cantidad de aplicaciones y datos que pueden estar activos simultáneamente.

ROM (Read-Only Memory): Es una memoria no volátil que almacena firmware y software esencial, como el BIOS o el sistema de arranque. A diferencia de la RAM, la ROM no se puede modificar fácilmente y retiene su contenido incluso sin energía.

Vigencia: Ambos términos siguen siendo vigentes, aunque las tecnologías han evolucionado. Por ejemplo, la RAM ahora incluye tipos como DDR4 y DDR5, mientras que la ROM ha dado paso a memorias flash (como las usadas en unidades SSD).

## 7. Opcode
El opcode (código de operación) es una parte fundamental de una instrucción de máquina que especifica la operación que la CPU debe realizar. Cada opcode corresponde a una operación específica, como sumar, restar, cargar datos o saltar a una dirección de memoria. El opcode es interpretado por la Unidad de Control, que genera las señales necesarias para ejecutar la operación.

Ejemplo: En una arquitectura simple, el opcode 0001 podría significar "sumar", mientras que 0010 podría significar "cargar datos".

Relación con los operandos: El opcode suele ir acompañado de operandos, que son los datos o direcciones sobre los que se realiza la operación.