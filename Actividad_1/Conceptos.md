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

# Funcionamiento del computador simulado

![Computador](<../Imagenes_Actividad_1/WhatsApp Image 2025-02-07 at 3.27.41 PM.jpeg>)

## Memoria ROM

Contiene el programa que ya fue predefinido el cual la CPU ejecutará.
Al iniciar la simulación, la CPU lee las instrucciones almacenadas en la ROM y las ejecuta.

![ROM](<../Imagenes_Actividad_1/WhatsApp Image 2025-02-07 at 3.02.26 PM.jpeg>)

## CPU (Unidad Central de Procesamiento)

Es el circuito encargado de interpretar y ejecutar las instrucciones del programa. Recibe las instrucciones desde la ROM y las ejecuta, interactuando con la memoria RAM y los dispositivos de entrada y salida.
Maneja señales de control, direcciones de memoria y escritura - lectura de datos.

![CPU](<../Imagenes_Actividad_1/WhatsApp Image 2025-02-07 at 3.02.41 PM.jpeg>)

## Memoria RAM (Memory)

Almacena los datos generados y modificados durante la ejecución del programa. En este caso, es la encargada de recibir entradas del teclado y actualizar la pantalla.

![Memoria RAM](<../Imagenes_Actividad_1/WhatsApp Image 2025-02-07 at 3.02.50 PM.jpeg>)

## Clock

Controla la velocidad con la que se ejecutan las instrucciones.
Sincroniza el flujo de datos entre los componentes.

![Reloj](<../Imagenes_Actividad_1/WhatsApp Image 2025-02-07 at 3.03.04 PM.jpeg>)

## Teclado

Actúa como entrada de usuario.
Al presionar una tecla, se envía una señal a la CPU, que luego actualiza la memoria y la pantalla.

![Teclado](<../Imagenes_Actividad_1/WhatsApp Image 2025-02-07 at 3.22.40 PM.jpeg>)

## Pantalla

Actúa como salida gráfica del sistema.
Cuando se presiona una tecla, la memoria cambia los valores correspondientes y la pantalla se actualiza, encendiendo píxeles en negro.
Al soltar la tecla, los píxeles vuelven a blanco, mostrando la interacción entre el usuario y el sistema.

![alt text](<../Imagenes_Actividad_1/WhatsApp Image 2025-02-07 at 3.25.14 PM.jpeg>)


# Preguntas

## 1. ¿Qué es un programa y dónde se almacena?

Un programa es un conjunto de instrucciones que una computadora puede ejecutar para realizar una tarea específica. Estas instrucciones están escritas en un lenguaje de programación y pueden ser interpretadas o compiladas en código máquina.

Los programas se almacenan en la memoria secundaria (como un disco duro o una unidad SSD) cuando no están en ejecución. Sin embargo, cuando se ejecutan, se cargan en la memoria RAM para que el procesador pueda acceder rápidamente a las instrucciones.

## 2. Si pongo un comentario en un programa como: //variable tipo contador, ¿dónde se almacena dicho comentario?

Los comentarios en un programa son parte del código fuente y se almacenan en el archivo del programa en la memoria secundaria (disco duro o SSD).

Sin embargo, cuando el código es compilado o interpretado, los comentarios no forman parte del programa ejecutable, ya que los compiladores e intérpretes los ignoran. Solo sirven como anotaciones para los programadores en el código fuente.

## 3. ¿Dónde se almacena una variable?

El almacenamiento de una variable depende del tipo de variable y del contexto en el que se usa:

Variables locales: Se almacenan en la pila (stack) de memoria. Son temporales y existen solo mientras la función o bloque de código donde fueron declaradas está en ejecución.
Variables globales y estáticas: Se almacenan en la sección de datos de la memoria RAM, y permanecen durante toda la ejecución del programa.
Variables dinámicas (asignadas con malloc en C o con new en C++ y otros lenguajes): Se almacenan en el montículo (heap), un área de memoria gestionada dinámicamente por el programador o el recolector de basura.

# Descripción del Fetch - Decode - Execute

## Fetch:
En esta etapa, la CPU busca la siguiente instrucción que debe ejecutar. Esta instrucción está almacenada en la memoria principal (RAM) en una dirección específica. El procesador usa un registro llamado Contador de Programa (PC) para saber dónde está esa instrucción. Una vez que la encuentra, la lleva a un lugar especial dentro de la CPU llamado Registro de Instrucción (IR).

## Decode:
Aquí, la CPU "traduce" la instrucción que acaba de buscar. Piensa en esto como descifrar un código: la instrucción está en un lenguaje que la CPU entiende (lenguaje máquina), pero necesita descomponerla para saber exactamente qué hacer. Por ejemplo, la CPU determina si la instrucción es una suma, una resta, o si necesita mover datos de un lugar a otro.

## Execute:
En esta última etapa, la CPU lleva a cabo la acción que indicó la instrucción. Por ejemplo, si la instrucción era sumar dos números, la CPU realiza la operación matemática. Si era mover datos, los transfiere de un lugar a otro. Una vez que termina, el ciclo se repite: la CPU busca la siguiente instrucción, la decodifica y la ejecuta.

##Instrucciones y características

### Resumen sobre los tipos de instrucciones del procesador del caso de estudio

El procesador del caso de estudio utiliza principalmente **instrucciones tipo C**, que son muy versátiles y permiten realizar una amplia variedad de operaciones. Estas instrucciones se caracterizan por tener una estructura específica en su codificación binaria, que define qué operación realizar, dónde almacenar el resultado y si se debe realizar un salto condicional o incondicional. A continuación, explico las características de estas instrucciones y cómo funcionan, junto con un ejemplo.

---

### **Estructura de las instrucciones tipo C**
Las instrucciones tipo C están compuestas por 16 bits, organizados de la siguiente manera:

1. **Bits 15-13:** Siempre son `111`, indicando que es una instrucción tipo C.
2. **Bits 12-6:** Especifican la operación a realizar (por ejemplo, suma, resta, AND, OR, etc.).
3. **Bits 5-3:** Indican el destino donde se almacenará el resultado (por ejemplo, registro D, registro A, memoria, etc.).
4. **Bits 2-0:** Determinan si se debe realizar un salto condicional o incondicional, basado en el resultado de la operación.

---

### **Características de las instrucciones tipo C**

1. **Operaciones:**  
   Las instrucciones tipo C pueden realizar operaciones aritméticas (suma, resta), lógicas (AND, OR, NOT), manipulación de datos (carga, almacenamiento) y saltos condicionales. Por ejemplo:
   - `D = A` (copia el valor del registro A al registro D).
   - `D = D + A` (suma los valores de los registros D y A, y almacena el resultado en D).
   - `D = D & A` (realiza una operación AND bit a bit entre D y A).

2. **Destinos:**  
   El resultado de la operación puede almacenarse en diferentes lugares, como:
   - El registro D.
   - El registro A.
   - La memoria en la dirección apuntada por A (`Memoria[A]`).
   - Una combinación de estos (por ejemplo, almacenar en D y en `Memoria[A]`).

3. **Saltos:**  
   Las instrucciones tipo C pueden modificar el flujo del programa mediante saltos condicionales o incondicionales. Por ejemplo:
   - `JGT` (salta si el resultado es mayor que 0).
   - `JEQ` (salta si el resultado es igual a 0).
   - `JMP` (salto incondicional).

---

### **Ejemplo de instrucción tipo C**

#### Instrucción: `0xEC10` (en binario: `1110 1100 0001 0000`)
- **Operación:** `D = A`  
  - Los bits `a c1 c2 c3 c4 c5 c6` son `0110000`, que corresponden a "leer el valor del registro A".
  - Los bits `d1 d2 d3` son `010`, que indican que el resultado se almacena en el registro D.
  - Los bits `j1 j2 j3` son `000`, lo que significa que no hay salto.

#### Explicación:
1. La CPU lee el valor del registro A.
2. Almacena ese valor en el registro D.
3. No se realiza ningún salto, por lo que el programa continúa con la siguiente instrucción.

---

### **Otro ejemplo: Instrucción con salto condicional**

#### Instrucción: `0xE305` (en binario: `1110 0011 0000 0101`)
- **Operación:** `D = D + 1; JNE`  
  - Los bits `a c1 c2 c3 c4 c5 c6` son `0011111`, que corresponden a "realizar D + 1".
  - Los bits `d1 d2 d3` son `010`, que indican que el resultado se almacena en el registro D.
  - Los bits `j1 j2 j3` son `101`, que corresponden a "salto si el resultado no es igual a 0" (`JNE`).

#### Explicación:
1. La CPU incrementa el valor del registro D en 1.
2. Si el nuevo valor de D no es 0, el programa salta a la dirección almacenada en el registro A.
3. Si el valor de D es 0, el programa continúa con la siguiente instrucción.

---

### **Conclusión**
Las instrucciones tipo C son fundamentales para el funcionamiento del procesador, ya que permiten realizar operaciones aritméticas, lógicas, manipulación de datos y control de flujo. Su estructura binaria está diseñada para ser flexible y eficiente, lo que permite implementar programas complejos con un conjunto reducido de instrucciones. Por ejemplo, la instrucción `D = A` es una operación sencilla pero esencial para mover datos entre registros, mientras que las instrucciones con saltos condicionales permiten implementar estructuras de control como bucles y condicionales. 

# Proceso de Decodificación de Instrucciones en la CPU

Identificación de los 16 bits de la instrucción

En el circuito de la CPU, la instrucción que ingresa es un dato de 16 bits que se encuentra etiquetado como instruction. Este bus se divide en los siguientes componentes según su significado y función:

`Bits 0-14`: Representan diferentes partes de la instrucción, dependiendo de si es una instrucción tipo A o tipo C.

`Bit 15`: Actúa como un identificador para el tipo de instrucción:

`0`: Indica una instrucción de tipo A.

`1`: Indica una instrucción de tipo C.

El circuito decodifica este bit para determinar el tipo de instrucción que debe procesarse.

Proceso de Decodificación

1. **Instrucción Tipo A**

**Identificación**: Cuando el bit más significativo (bit 15) es 0, el circuito interpreta la instrucción como tipo A.

**Propósito**:

Cargar un valor inmediato en el registro A.

**Flujo**:

Los bits 0-14 se envían directamente al registro A.

No se utilizan señales relacionadas con la ALU ni con registros D o memoria de datos.

2. **Instrucción Tipo C**

Identificación: Cuando el bit más significativo (bit 15) es 1, el circuito interpreta la instrucción como tipo C.

**Propósito**:

Realizar operaciones aritméticas o lógicas con la ALU.

Controlar los registros `D`, `A`, y la memoria.

**Flujo**:

Los bits 0-5 configuran las señales de control de la ALU (`zx`, `nx`, `zy`, `ny`, `f`).

Los bits 6-11 especifican los destinos del resultado (`destD`, `destA`, `writeM`).

Los bits 12-14 determinan las condiciones de salto (`jmpGt`, `jmpEq`, `jmpLt`).

# Evidencia para el repositorio:
1. **Objetivo del programa**:
   - Este programa implementa un ciclo que suma los números enteros desde 1 hasta 100 y almacena el resultado en la variable sum.

2. **Ejecución paso a paso**:
   - Inicialización:
       - `i` se establece en 1.
       - `sum` se inicializa en 0.
   - Ciclo:
       - Se resta el valor actual de `i` a 100.
       - Si el resultado es menor o igual a 0 (`JLE`), el programa salta a la etiqueta `(END)`.
       - En cada iteración, el valor de `i` se suma a `sum`.
       - Incrementa `i` en 1.
       - Salta al inicio del ciclo.
   - Fin del programa:
       - Al alcanzar la condición `i > 100`, el programa se detiene en la etiqueta `(END)`.

3. **Funcionamiento de la CPU**:
   - La CPU ejecuta instrucciones en un ciclo de búsqueda, decodificación y ejecución.
   - El contador de programa (PC) controla la dirección de la instrucción actual.
   - Los registros (`A`, `D`, `M`) trabajan en conjunto para manipular datos.
   - La ALU realiza las operaciones matemáticas y lógicas (por ejemplo, suma, comparación).

4. **Opciones de animación exploradas**:
   - Fetch/Execute Cycle: Permite observar cómo la CPU extrae y ejecuta cada instrucción.
   - ALU Operations: Muestra los cálculos realizados por la unidad aritmética y lógica.
   - Memory Updates: Visualiza los cambios en los registros y la memoria principal.

**Resultado**:
- Al ejecutar el programa, se puede observar cómo la CPU suma iterativamente los valores de `i` hasta alcanzar 100, almacenando el resultado en `sum`.
- La animación destaca los pasos precisos de la CPU, como el uso de registros y las decisiones basadas en las comparaciones de la ALU.
  
