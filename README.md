# Arquitectura-ARM
Investigacion sobre la Arquitectura ARM TEAM-3-2025-1

# Historia de Arm
Arm comenzo en la decada de 1980 en Cambridge, Inglaterra, cuando Acorn Computers Ltd. buscaba un procesador mas potente para competir con los PC de IBM. En 1983, los ingenieros Sophie Wilson y Steve Furber iniciaron el desarrollo de la arquitectura Acorn RISC Machine (ARM), basandose en estudios de Stanford y Berkeley sobre procesadores RISC.

En 1985, VLSI Technology fabrico el primer procesador ARM1, disenado con 808 lineas de codigo en Basic. Un año despues, en 1986, surgio el ARM2, el primer chip comercial de la compania. Destacaba por su bajo consumo de energia y su eficiencia, superando al Intel 80286 a pesar de tener solo 30,000 transistores.

Nacimiento de ARM Ltd
En 1990, se fundo Advanced RISC Machines Ltd (ARM Ltd.) con la colaboracion de:

Acorn Computers (aporto ingenieros)
Apple Computer (financiamiento)
VLSI Technology (herramientas de desarrollo)
En 1993, Apple lanzo el Newton, un dispositivo pionero en computacion movil con procesador ARM, y la compania establecio una alianza con Texas Instruments, validando su modelo de negocio basado en licencias.

Expansion al mercado movil
En 1994, ARM presento el ARM7TDMI, introduciendo la tecnologia Thumb para optimizar el uso de instrucciones en dispositivos con recursos limitados. Su adopcion en el Nokia 6110 impulso su exito, alcanzando mas de 10 mil millones de unidades fabricadas.

Evolucion tecnologica
A lo largo de los años, ARM ha lanzado nuevas generaciones de procesadores:

- **ARMv5 (1999):** Mejor eficiencia y rendimiento.  
- **ARM9, ARM10 y ARM11:** Avances en procesamiento.  

**Familia Cortex:**  
  - **Cortex-A:** Alto rendimiento.  
  - **Cortex-R:** Tiempo real.  
  - **Cortex-M:** Bajo consumo.  

Arm en la actualidad
En 2017, SoftBank adquirio la empresa y cambio su nombre de ARM a Arm, manteniendo su estrategia de licenciamiento. Actualmente, sus procesadores estan en millones de dispositivos, desde telefonos y tablets hasta servidores y sistemas embebidos. Su enfoque en eficiencia energetica, rendimiento y bajo costo ha sido clave en la revolucion de la computacion movil.

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

# Anexos

## Flujo de trabajo

### Evitar conflictos
* Realizar git pull antes de realizar cambios o hacer push
* no modificar los mismos archivos a la vez o almenos las mismas lineas
* no trabajar en la misma rama de manera simultanea
* tener una buena comunicacion en el equipo de trabajo para coordinar cambios