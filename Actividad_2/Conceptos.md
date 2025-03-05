# Actividad 2 - Mapa de memoria y tipos de arquitectura

## 1. ¿Qué es y para qué sirve el mapa de memoria de un microprocesador?
El mapa de memoria de un microprocesador es una representación gráfica o estructural que muestra cómo está organizada la memoria del sistema. Este mapa indica:
- Las direcciones de memoria disponibles.
- Los dispositivos conectados al sistema.
- Las áreas reservadas para programas o datos.

### Propósito:
- Permitir al programador o diseñador comprender y controlar el acceso a los diferentes componentes de memoria.
- Asegurar una gestión eficiente y evitar conflictos en el uso de la memoria.

---

## 2. Basándote en la figura 3, responde:

### a. ¿Cuántos pines del bus de direcciones del MC6802 se utilizan en esta conexión? ¿Cuáles son los nombres utilizados para representarlos?
- **Pines utilizados:** 16 pines del bus de direcciones.
- **Nombres:** A0 a A15.

### b. ¿De qué valor es la memoria total de almacenamiento del MC6846? Incluye los cálculos que realizaste.
- El bus de direcciones es de 16 bits, por lo que la memoria total se calcula como:
  
  \( 2^{16} = 65,536 \) bytes (64 KB).

### c. ¿Cuántos bits ocupa cada dato al que se puede acceder en la memoria MC6846? ¿Cómo lo dedujiste?
- **Dato por acceso:** 8 bits (1 byte).
- **Justificación:** El MC6846 utiliza un bus de datos de 8 bits, lo que implica que cada dato ocupa 1 byte.

---

## 3. ¿Cuáles son las características más relevantes de la arquitectura von Neumann y Harvard?

### Arquitectura von Neumann:
- Comparte un único bus para acceder tanto a las instrucciones como a los datos.
- Puede ocurrir el fenómeno de "cuello de botella de von Neumann".
- Diseño más simple con menos hardware.
- Común en computadoras de propósito general.

### Arquitectura Harvard:
- Utiliza buses separados para instrucciones y datos, permitiendo acceso simultáneo.
- Mejor rendimiento al evitar conflictos de acceso.
- Común en sistemas embebidos y aplicaciones de tiempo real.
- Requiere diseño más complejo y hardware adicional.

---

## 4. ¿Cuáles son las características más relevantes de la arquitectura CISC y RISC?

### CISC (Complex Instruction Set Computer):
- Conjunto de instrucciones amplio y complejo.
- Reduce la cantidad de instrucciones necesarias para completar una tarea.
- Ideal para aplicaciones con espacio de memoria limitado.
- Ejemplo: Procesadores x86.

### RISC (Reduced Instruction Set Computer):
- Conjunto de instrucciones reducido y optimizado para operaciones simples.
- Instrucciones de longitud fija y un ciclo de reloj por instrucción.
- Más eficiente en términos de rendimiento y consumo energético.
- Ejemplo: Procesadores ARM.

---

## 5. ¿Cuál es tu opinión sobre los tipos de arquitecturas que se observan en los microprocesadores? (RESPUESTA COMO ESTUDIANTE)

Desde mi perspectiva como estudiante, cada tipo de arquitectura tiene su propio campo de aplicación y ventajas:

- **Arquitecturas von Neumann y Harvard:** La simplicidad de von Neumann lo hace ideal para computadoras generales, mientras que la arquitectura Harvard destaca en sistemas embebidos y aplicaciones que demandan eficiencia y velocidad.
- **Arquitecturas CISC y RISC:** La arquitectura RISC representa una evolución hacia diseños más eficientes, ideales para dispositivos modernos como smartphones. Por otro lado, CISC sigue siendo relevante en computadoras de propósito general debido a su capacidad para manejar instrucciones complejas.

En conclusión, la elección depende de los requerimientos específicos del sistema y el entorno en el que se utilice.

## Análisis de la conexión MC6802 y MC6846

### 1. Pines del bus de direcciones utilizados
- **Cantidad de pines utilizados:** 11
- **Nombres de los pines:** A0 a A10

---

### 2. Memoria total de almacenamiento del MC6846
- **Memoria:** 2 KB de memoria ROM

#### Cálculo:
```
2 KB = 2 × 1024 = 2048 bytes
```
> **Resultado:** La memoria total de almacenamiento del MC6846 es de **2048 bytes**.

---

### 3. Tamaño de cada dato accesible en la memoria del MC6846
- **Tamaño de cada dato:** 8 bits (1 byte)

#### Deducción:
El bus de datos compartido entre el MC6802 y el MC6846 está etiquetado como **D0-D7**, lo que indica que el bus de datos es de **8 bits**. Por lo tanto, cada acceso a la memoria del MC6846 corresponde a un dato de **1 byte (8 bits)**.

¿Cuál crees que sea la arquitectura de los procesadores que has analizado hasta aquí? ¿Arquitectura von Newman o arquitectura Harvard?

## Procesadores y su arquitectura

### MC6802 y MC6808
`MC6802` = Arquitectura von Neumann: Comparte el mismo espacio de direcciones para instrucciones y datos, aunque las líneas de datos y direcciones estén separadas físicamente.
`MC6808` = Arquitectura von Neumann: Similar al MC6802, comparten el espacio de direcciones para instrucciones y datos.

### 8086
`Intel8086` = Arquitectura von Neumann: Las instrucciones y los datos comparten el mismo espacio de memoria. La multiplexación del bus es solo un mecanismo de optimización.

