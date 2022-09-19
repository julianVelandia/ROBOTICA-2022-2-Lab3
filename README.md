# Laboratorio 3
## Robótica - Universidad Nacional De Colombia - Sede Bogotá
### Sebastian Cubides - Julián Velandia
***
* Código en RAPID del módulo utilizado para el desarrollo de la práctica:
    Para la realización de las tareas propuestas en la guía de laboratorio se utilizó el desarrollo hecho previamente para el laboratorio 1 y se modificaron las instrucciones del código RAPID para leer las entradas digitales y emitir salidas digitales.
    
    Para recibir las entradas digitales (Botones en el panel del controlador) se configuró la instrucción WaitDI (Digital Input),1 , la cual espera a que la entrada en cuestión tome un valor lógico 1 y luego procede a ejecutar el código inmediatamente subsecuente.
    
    Para emitir las señales digitales (Luces de aviso del panel del controlador) se usó la instrucción DO (Digital Output),0 para iniciar todas en estado lógico bajo y luego DO (Digital Output),1 para llevarlas a un estado alto.