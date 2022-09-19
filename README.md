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