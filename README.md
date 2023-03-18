# Problema_Concurrencia
Entrega de la primera semana de sistemas operativos, problema numero 1
# Semáforos binarios y enteros

Los semáforos son una herramienta clave para la coordinación y sincronización de los recursos compartidos entre procesos en los sistemas operativos. Hay dos tipos principales de semáforos: binarios y enteros.

- Los **semáforos binarios** tienen solo dos valores posibles: 0 o 1. Se usan para permitir el acceso a un recurso compartido por un proceso a la vez.

- Los semáforos enteros pueden tener valores positivos o cero. Se utilizan para permitir el acceso a un recurso compartido por múltiples procesos, pero solo uno a la vez.

Ambos tipos de semáforos son importantes para asegurar que los procesos trabajen de manera ordenada y sin interferencias en un sistema operativo.

## Relación entre los semáforos y la sincronización

Los semáforos son una herramienta clave para la sincronización de procesos en sistemas operativos. La sincronización implica coordinar los procesos para evitar conflictos al acceder a los recursos compartidos.

- Los semáforos permiten a los procesos acceder a los recursos compartidos de forma ordenada y controlada. Por ejemplo, un semáforo puede indicar si un recurso está disponible o no. Si el recurso está ocupado, el proceso que lo solicita puede bloquearse y esperar a que esté disponible.

Además, los semáforos también permiten establecer reglas de acceso a los recursos compartidos, como la exclusión mutua, para asegurar que solo un proceso acceda al recurso a la vez.

En conclusión, los semáforos son una herramienta importante para la sincronización de procesos en sistemas operativos, ya que ayudan a establecer reglas de acceso para evitar conflictos o inconsistencias en el acceso a los recursos compartidos.
