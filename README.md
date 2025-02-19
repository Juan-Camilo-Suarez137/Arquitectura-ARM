
# Arquitectura-ARM
Investigacion sobre la Arquitectura ARM TEAM-3-2025-1

# Introduccion de la Arquitectura ARM 

La arquitectura ARM (Advanced RISC Machine) es una de las arquitecturas de microprocesadores más influyentes y ampliamente utilizadas 
en el mundo de la computación moderna. Desde su creación en la década de 1980, ARM ha evolucionado significativamente, adaptándose a 
las necesidades cambiantes de la tecnología y del mercado.
Se caracteriza por ser más sencilla y directa en comparación con las complejas instrucciones de los procesadores x86 tradicionales. 
Esta simplicidad se traduce en un consumo de energía significativamente menor y, por ende, en una mayor eficiencia energética, 
lo que ha sido un factor clave en su predominio en el mercado de dispositivos móviles y sistemas embebidos.

La capacidad de los procesadores ARM para realizar operaciones con menos ciclos de reloj y una gestión de energía más eficiente ha 
sido fundamental para su éxito en dispositivos donde la conservación de la batería es crucial. Además, su arquitectura permite una 
integración más fácil con otros tipos de tecnologías, lo que facilita el desarrollo de sistemas más compactos y con mejor rendimiento energético.

En los últimos años, ARM ha comenzado a expandirse más allá de su nicho tradicional en dispositivos móviles y embebidos. En el mundo de los servidores
 y los sistemas de cómputo de alto rendimiento, ARM está ofreciendo alternativas viables a las arquitecturas x86, especialmente en aplicaciones que requieren 
 una gran cantidad de procesamiento paralelo. Este movimiento hacia servidores y centros de datos se debe en parte a su capacidad para manejar múltiples tareas 
 de manera eficiente, reduciendo así los costos operativos y la huella de carbono de estos centros.

 La infraestructura ARM también está siendo adoptada en el campo de la inteligencia artificial y el aprendizaje automático, donde la eficiencia en el procesamiento
  de grandes volúmenes de datos es esencial. Su habilidad para realizar cálculos complejos con menor consumo de energía la convierte en una opción atractiva para 
  desarrollar soluciones de IA más sostenibles y económicamente viables.
  
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

# Registro

*¿Qué es?*

Los registros en la arquitectura ARM son ubicaciones de almacenamiento especiales dentro del proceso que pueden contener valores temporales y direcciones de memoria. La arquitectura ARM es ampliamente utilizada en dispositivos electrónicos como teléfonos inteligentes, tables y automóviles.

*Características* 

1)	Se especifican en las instrucciones ARM. 
2)	Usan 4 bist, lo que puede representar 16 registros. 
3)	Los nombres mnemotécnicos se especifican como RO a R15. 
4)	SP, LR y PC son alias para R13, R14 y R15.
5)	ARM recomienda usar los nombres PS, LR y PC en lugar de R13, R14 y R15.

*Usos de los registros ARM* 

1)	El procesador ARM solo entiende el valor dado utilizando 4 bits en la mayoría de las instrucciones.
2)	Los registros de configuración controlan el comportamiento de algún elemento o periférico del sistema.
*Funciones de los registros ARM* 

1)	El R15 se usa como contador de programa o pc 
2)	El R14 se usa para almacenar la dirección de retomar cuando se llama a una subrutina o se genera una excepción.
3)	El R13 es el stack Pointe


**Código Ejemplo**
código de ejemplo en ensamblador ARM que imprime "¡Hola, ARM!" en la consola. Este código está diseñado para ARMv7 (32 bits) y puede ejecutarse en un entorno Linux con QEMU y un ensamblador como as y ld.

🔹 Código en ensamblador ARM (ARMv7 - 32 bits)
assembly
Copiar
Editar
.global _start      @ Define el punto de entrada

.section .data
mensaje: .asciz "¡Hola, ARM!\n"  @ Mensaje a imprimir

.section .text
_start:
    @ Llamada al sistema write (sys_write)
    mov r0, #1            @ File descriptor (1 = salida estándar)
    ldr r1, =mensaje      @ Dirección del mensaje
    ldr r2, =13           @ Longitud del mensaje
    mov r7, #4            @ Número de syscall (4 = sys_write)
    svc #0                @ Llamada al sistema

    @ Llamada al sistema exit (sys_exit)
    mov r0, #0            @ Código de salida
    mov r7, #1            @ Número de syscall (1 = sys_exit)
    svc #0                @ Llamada al sistema
🔹 Explicación del código
Definimos el mensaje "¡Hola, ARM!\n" en la sección .data.
Llamamos a la syscall write para imprimir el mensaje en la consola.
r0 = 1 (salida estándar)
r1 = mensaje (dirección del mensaje)
r2 = 13 (longitud del mensaje)
r7 = 4 (sys_write en Linux)
svc #0 (invoca la llamada al sistema)
Llamamos a exit para terminar el programa.
🔹 Cómo compilar y ejecutar (en Linux)
Si tienes arm-linux-gnueabi-gcc y qemu-arm instalados, puedes hacer lo siguiente:

sh
Copiar
Editar
as -o hola_arm.o hola_arm.s         # Ensamblar el código
ld -o hola_arm hola_arm.o            # Enlazar
qemu-arm ./hola_arm                  # Ejecutar en QEMU
📌 Salida esperada en la consola:

Copiar
Editar
¡Hola, ARM!

# Aplicacion

Debido a su amplia aplicabilidad, los procesadores ARM se utilizan en casi todos los entornos industriales:


Teléfonos inteligentes y tabletas: ARM lidera los mercados de teléfonos inteligentes y tabletas principalmente por sus ventajas de bajo consumo de energía y altos niveles de rendimiento.

Dispositivos IoT: los electrodomésticos inteligentes, los dispositivos portátiles inteligentes y los dispositivos IoT similares prefieren insertar un procesador ARM por razones como el menor consumo de energía, la alta escalabilidad y una variedad de productos disponibles en el mercado.


Sistemas integrados: una arquitectura ARM es adecuada para la mayoría de los sistemas integrados en el sector automotriz, equipos médicos y controles industriales.


Computadoras portátiles y servidores: corporaciones como Apple han comenzado a utilizar procesadores basados ​​en ARM en MacBooks. AWS está proporcionando instancias basadas en ARM dentro de su infraestructura en la nube .

Dispositivos portátiles: los procesadores ARM tienen una alta eficiencia con un bajo consumo de energía, lo que permite
La capacidad de los procesadores ARM para realizar operaciones con menos ciclos de reloj y una gestión de energía más eficiente ha 
sido fundamental para su éxito en dispositivos donde la conservación de la batería es crucial. Además, su arquitectura permite una 
integración más fácil con otros tipos de tecnologías, lo que facilita el desarrollo de sistemas más compactos y con mejor rendimiento energético.

En los últimos años, ARM ha comenzado a expandirse más allá de su nicho tradicional en dispositivos móviles y embebidos. En el mundo de los servidores y los sistemas de cómputo de alto rendimiento, ARM está ofreciendo alternativas viables a las arquitecturas x86, especialmente en aplicaciones que requieren una gran cantidad de procesamiento paralelo. Este movimiento hacia servidores y centros de datos se debe en parte a su capacidad para manejar múltiples tareas de manera eficiente, reduciendo así los costos operativos y la huella de carbono de estos centros.
La infraestructura ARM también está siendo adoptada en el campo de la inteligencia artificial y el aprendizaje automático, donde la eficiencia en el procesamiento de grandes volúmenes de datos es esencial. Su habilidad para realizar cálculos complejos con menor consumo de energía la convierte en una opción atractiva para  desarrollar soluciones de IA más sostenibles y económicamente viables.

