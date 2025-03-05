# Preguntas y Respuestas sobre Instrucciones ARM

## 1. Explica la diferencia entre desplazamiento lógico y desplazamiento aritmético con tus propias palabras.
- **Desplazamiento lógico (LSR o LSL)**: Mueve los bits hacia la derecha (LSR) o izquierda (LSL), rellenando con ceros en la posición vacía. No conserva el signo.
- **Desplazamiento aritmético (ASR)**: Mueve los bits hacia la derecha, pero mantiene el bit de signo original, útil para operar con números negativos.

## 2. ¿En qué tipo de aplicaciones sería más útil usar ASR en lugar de LSR?
- ASR es útil en operaciones con números negativos representados en complemento a dos, como divisiones por potencias de 2, ya que conserva el signo.

## 3. Explica la diferencia entre `MOV R0, #42` y `MOV R0, R1`.
- `MOV R0, #42` mueve un valor inmediato (42) al registro R0.
- `MOV R0, R1` copia el valor de R1 en R0.

## 4. ¿Qué función tiene la instrucción `MOVS` y cómo difiere de `MOV`?
- `MOVS` es igual a `MOV`, pero actualiza los **flags** del procesador (N, Z, C, V), útil para evaluar condiciones en instrucciones posteriores.

## 5. ¿Por qué se utiliza la instrucción `MOVT` en combinación con `MOVW`?
- `MOVW` carga la parte baja de un registro (16 bits) y `MOVT` la parte alta (otros 16 bits), permitiendo cargar valores de 32 bits en dos instrucciones.

## 6. ¿Por qué algunos valores se pueden mover de manera inmediata y otros no?
- ARM tiene restricciones en los valores inmediatos, ya que solo puede codificar ciertos patrones de 8 bits rotados dentro de un registro de 32 bits.

## 7. ¿Cuál es el máximo valor que puede utilizarse como valor inmediato (#valor)?
- En la mayoría de las arquitecturas ARM, el valor inmediato máximo depende del formato de codificación, generalmente **8 bits rotados**, lo que da un rango no lineal.

## 8. ¿Cuál es la alternativa para mover números grandes de forma inmediata?
- Se usa `MOVW` + `MOVT` o se carga el valor desde memoria mediante `LDR`.
