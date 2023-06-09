Jeyllon Sandoval 2021-1155

Emmanuel Torres 2021-1097


# Problema Concurrencia

## Que es la concurrencia?

La **concurrencia** se refiere a las situaciones en las que dos o más procesos puedan coincidir en el acceso a un recurso compartido o que requieran coordinarse en su ejecución. Para evitar dicha coincidencia, el sistema operativo ofrece mecanismos de arbitraje que permiten coordinar la ejecución de los procesos.

> En **sistemas multiprocesador**, esta ejecución simultanea podría conseguirse completamente, ya que podremos asignarle un proceso a un procesador en específico. Pero en un **sistema de un procesador** se produce un intercalado (interpuesto) de las instrucciones de los procesos en ejecución (es decir ejecución simultanea de ambos procesos). 


## Concepto básico de semáforo en los sistemas operativos 

Un **semáforo** en **sistemas operativos** es una herramienta que ayuda a diferentes procesos o hilos a compartir recursos de manera organizada y segura. 

- Es como una señal que indica si un **recurso** está disponible o no para su uso. 

> Los **semáforos** se utilizan para evitar que varios procesos o hilos accedan al mismo **recurso** al mismo tiempo, lo que puede causar errores. 

Hay diferentes tipos de **semáforos**, algunos con dos valores posibles y otros con valores numéricos, pero todos se utilizan para controlar el acceso a recursos compartidos. 
> Los semáforos son importantes en la programación para que los procesos o hilos cooperen y usen los recursos de manera eficiente.


## Semáforos binarios y enteros

Los **semáforos** son una herramienta clave para la coordinación y sincronización de los recursos compartidos entre procesos en los sistemas operativos.

>Un semáforo (s) es una variable que, aparte de la inicialización, solo se puede acceder por medio de 2 operaciones atómicas y mutuamente exclusivas:
>> Una operacion atomica eses una operación en la que un procesador puede simultáneamente leer una ubicación y escribirla en la misma operación del bus. Esto previene que cualquier otro procesador o dispositivo de E/S escriba o lea la memoria hasta que la operación se haya completado.
>>El término atómico implica la indivisibilidad e irreductibilidad del proceso, ya que este debe realizarse en su totalidad o en caso de ser interrumpido poder deshacer sus acciones de modo que fuese como si no se hubiese realizado acción alguna.
>
>
>Wait(s): Referenciada normalmente como P(s) o Down(s). Si el estado indica cero, el proceso se queda atrapado en el semáforo hasta que sea despertado por otro proceso. Si el estado indica que un proceso más puede acceder el recurso se decrementa el contador y la operación termina con exito.
>
>Signal(s): Referenciada normalmente como V(s), Up(s), Post(s) o Release(s). Una vez se ha terminado el uso del recurso, el proceso lo señaliza al semáforo. Si queda algún proceso bloqueado en el semáforo uno de ellos sea despertado, sino se incrementa el contador. La operación signal() también tiene que estár implementada como instrucción atómica. En algunás implementaciones es posible comprobar si se haya despertado un proceso con exito en caso que hubiera alguno bloqueado.



Hay dos tipos principales de semáforos: binarios y enteros.

- Los **semáforos binarios** tienen solo dos valores posibles: 0 o 1. Se usan para permitir el acceso a un recurso compartido por un proceso a la vez.

- Los **semáforos enteros** pueden tener valores positivos o cero. Se utilizan para permitir el acceso a un recurso compartido por múltiples procesos, pero solo uno a la vez.

     ![Semaforo](/assests/images/Image4107.gif)

Ambos tipos de semáforos son importantes para asegurar que los procesos trabajen de manera ordenada y sin interferencias en un sistema operativo.

## Relación entre los semáforos y la sincronización

Los **semáforos** son una herramienta clave para la sincronización de procesos en **sistemas operativos**. La sincronización implica coordinar los procesos para evitar conflictos al acceder a los recursos compartidos.

- Los semáforos permiten a los procesos acceder a los recursos compartidos de forma ordenada y controlada. Por ejemplo, un semáforo puede indicar si un recurso está disponible o no. Si el recurso está ocupado, el proceso que lo solicita puede bloquearse y esperar a que esté disponible.

> Además, los semáforos también permiten establecer reglas de acceso a los recursos compartidos, como la exclusión mutua, para asegurar que solo un proceso acceda al recurso a la vez.

En conclusión, los semáforos son una herramienta importante para la sincronización de procesos en sistemas operativos, ya que ayudan a establecer reglas de acceso para evitar conflictos o inconsistencias en el acceso a los recursos compartidos.
