
¿Qué es?
Los registros en la arquitectura ARM son ubicaciones de almacenamiento especiales dentro del proceso que pueden contener valores temporales y direcciones de memoria. La arquitectura ARM es ampliamente utilizada en dispositivos electrónicos como teléfonos inteligentes, tables y automóviles.
Características 
1)	Se especifican en las instrucciones ARM. 
2)	Usan 4 bist, lo que puede representar 16 registros. 
3)	Los nombres mnemotécnicos se especifican como RO a R15. 
4)	SP, LR y PC son alias para R13, R14 y R15.
5)	ARM recomienda usar los nombres PS, LR y PC en lugar de R13, R14 y R15.
Usos de los registros ARM 
1)	El procesador ARM solo entiende el valor dado utilizando 4 bits en la mayoría de las instrucciones.
2)	Los registros de configuración controlan el comportamiento de algún elemento o periférico del sistema.
Funciones de los registros ARM 
1)	El R15 se usa como contador de programa o pc 
2)	El R14 se usa para almacenar la dirección de retomar cuando se llama a una subrutina o se genera una excepción.
3)	El R13 es el stack Pointer  
