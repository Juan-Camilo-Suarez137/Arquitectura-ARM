# Arquitectura-ARM
Investigacion sobre la Arquitectura ARM TEAM-3-2025-1

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