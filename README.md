# Laboratorio 3
## Robótica - Universidad Nacional De Colombia - Sede Bogotá
### Sebastian Cubides - Julián Velandia
***
* Código en RAPID del módulo utilizado para el desarrollo de la práctica:

    Para la realización de las tareas propuestas en la guía de laboratorio se utilizó el desarrollo hecho previamente para el laboratorio 1 y se modificaron las instrucciones del código RAPID para leer las entradas digitales y emitir salidas digitales.
    
    Para recibir las entradas digitales (Botones en el panel del controlador) se configuró la instrucción WaitDI (Digital Input),1 , la cual espera a que la entrada en cuestión tome un valor lógico 1 y luego procede a ejecutar el código inmediatamente subsecuente.
    
    Para emitir las señales digitales (Luces de aviso del panel del controlador) se usó la instrucción setDO (Digital Output),0 para iniciar todas en estado lógico bajo y luego setDO (Digital Output),1 para llevarlas a un estado alto.
    
    Las entradas se definieron como 2 de los botones del panel del controlador:
    
    - Uno de ellos lleva al robot a una posición articular de (-90,0,0,0,0,0), en la cual se permite al usuario una pose adecuada para colocar la herramienta.
    
    - El otro botón se configuró para que el robot realice la secuencia Home, Posición Media, Rutina de Dibujo, Posición Media, Home. (La rutina de dibujo consta en seguir la trayectoria para la letra J, unicamente)
    
    Las salidas se asignaron a 2 de las luces de indicación del panel del controlador:
    
    - Una de ellas se mantiene encendida siempre y cuando el robot no esté en la posición de colocar herramienta.
    
    - La otra se enciende cada vez que el robot va a ejecutar la secuencia para dibujar en el tablero, con el fin de indicar el funcionamiento.
    
    Finalmente se puede consultar el código realizado en la carpeta *YYY4*, adjunta en el repositorio.
    
***

* Videos del Funcionamiento:

    [![Alt text](https://img.youtube.com/vi/4ulQzXr5LVQ/0.jpg)](https://www.youtube.com/watch?v=4ulQzXr5LVQ)
    
    [![Alt text](https://img.youtube.com/vi/xCUMJ9VfpgM/0.jpg)](https://www.youtube.com/watch?v=xCUMJ9VfpgM)
    

***

* Descripción de la Solución:

    Como ya se ha comentado y evidenciado en los literales anteriores, la solución consistió en sincronizar los 2 botones, para colocar el robot en la posición herramienta y para ejecutar la secuencia de dibujo, y en sincronizar las 2 luces de aviso para indicar la operación que se esté realizando.
    
    Adicionalmente, se evidenció con la realización de la práctica, la necesidad de empezar a usar instrucciones lógicas más complejas, pues con las configuraciones asignadas, el robot debía siempre realizar las rutinas secuencialmente, por ejemplo, si se deseaba ir a la posición de herramienta, era necesario primero hacer el recorrido de la trayectoria en vacío.
    
    
    
    
    