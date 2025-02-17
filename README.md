# Arquitectura-ARM
Investigacion sobre la Arquitectura ARM TEAM-3-2025-1

# Ensambador

El lenguaje ensamblador para la arquitectura ARM es un lenguaje de programación de bajo nivel que permite a los desarrolladores escribir instrucciones que interactúan directamente con el hardware del procesador ARM. A diferencia de los lenguajes de alto nivel, el ensamblador ofrece un control preciso sobre los recursos del sistema, lo que es esencial en aplicaciones donde el rendimiento y la eficiencia son críticos, como en sistemas embebidos y dispositivos móviles.

## Características del Lenguaje Ensamblador ARM
1. Dependencia de la Arquitectura: El código ensamblador ARM está diseñado específicamente para la arquitectura ARM, lo que significa que las instrucciones están adaptadas a las particularidades de sus procesadores.

2. Instrucciones Simples y Eficientes: Las instrucciones en ensamblador ARM suelen ser simples y se ejecutan en un ciclo de reloj, lo que contribuye a la eficiencia energética y al rendimiento, características clave de los procesadores ARM.

3. Conjunto de Instrucciones RISC: ARM utiliza un conjunto de instrucciones reducido (RISC), lo que simplifica el diseño del procesador y permite una ejecución más rápida de las instrucciones.

4. Modos de Operación: Los procesadores ARM pueden operar en diferentes modos, como el modo usuario, sistema y supervisor, permitiendo gestionar distintos niveles de privilegio y acceso a recursos.

## Estructura Básica de un Programa en Ensamblador ARM
Un programa típico en ensamblador ARM se compone de las siguientes secciones:

- .text: Contiene el código ejecutable.

- .data: Almacena datos inicializados.

- .bss: Reserva espacio para datos no inicializados.

## Conjunto de Instrucciones ARM
El conjunto de instrucciones ARM incluye diversas categorías, entre las cuales destacan:

1. Instrucciones de Transferencia de Datos: Permiten mover datos entre registros y memoria.

    - LDR: Carga un valor desde la memoria a un registro.

    - STR: Almacena un valor de un registro en la memoria.

2. Instrucciones Aritméticas y Lógicas: Realizan operaciones matemáticas y lógicas.

    - ADD: Suma dos valores.

    - SUB: Resta dos valores.

    - MUL: Multiplica dos valores.

    - AND, ORR, EOR: Operaciones lógicas AND, OR y XOR.

3. Instrucciones de Control de Flujo: Gestionan el flujo de ejecución del programa.

    - B: Salto incondicional a una etiqueta.

    - BL: Llama a una subrutina.

    - BX: Cambia el flujo de ejecución a la dirección especificada en un registro.

4. Instrucciones de Comparación: Comparan valores y establecen banderas para decisiones condicionales.

    - CMP: Compara dos registros.

    - TST: Realiza una operación AND y establece banderas sin almacenar el resultado.

## Modos de Direccionamiento
ARM soporta varios modos de direccionamiento para acceder a los operandos:

Direccionamiento Inmediato: El operando es un valor constante dentro de la instrucción.

- Ejemplo: MOV r0, #10 // Mueve el valor 10 al registro r0.
    - Direccionamiento Registrado: El operando es el contenido de un registro.

- Ejemplo: MOV r1, r2 // Copia el valor de r2 en r1.
    - Direccionamiento Directo: La instrucción contiene la dirección de memoria donde se encuentra el operando.

- Ejemplo: LDR r3, [r4] // Carga en r3 el valor en la dirección apuntada por r4.
    - Direccionamiento Indirecto: La dirección efectiva se calcula sumando un desplazamiento al contenido de un registro.