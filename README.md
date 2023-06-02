# Proyecto_Sistemas_DigitalesII_Skeball
Juego Skeball programado para interactuar con un dispositivo de captura diseñado con ESP32.
Nombre del juego: Skeball virtual
Propósito del juego: Entregable final para la materia de sistema digitales II del programa de ingeniería electrónica.
Objetivo del juego: Los jugadores tomaran turnos para lanzar hasta 5 bolas y anotarlas en cualquiera de las dianas predispuestas en el juego. El jugados que al terminar sus lanzamientos consiga más puntos será el ganador.
Instrucciones del juego:

Abrir el archivo "index" usando google chrome y un computador.
Conectar el mando con el computador presionando el botón Connect BT Device que se encuentra en la esquina superior izquierda de la pantalla.
Para mover la dirección de tiro gire el control de izquierda a derecha.
Para aumentar la fuerza del tiro levante la punta del control hacia arriba
Para disminuir la fuerza del tire baje la punta del control
Para dispara su tiro presiones el botón "fire".
Para pausar el juego presione el botón "pause"
Cuando un jugador agote sus tiros el juego se reinicia automáticamente.
Descripción de mando (en esta sección deberán dar detalles técnicos de cómo está diseñado y construido el mando inalámbrico. Deben incluir también una imagen con el circuito electrónico).
El control esta construido con un microcontrolador ESP32 - Devkitv1 conectado con un acelerómetro MPU 6050. Los pines SCL y SCD del acelerómetro se conectan a los pines d22 y d21 de la ESP32 respectivamente. Los pines VCC y GND del acelerómetro y la ESP32 se conectan en paralelo. El acelerómetro mide el cambio del valor de posición en x, y, z; la ESP32 se encarga de calcular la fuerza y desplazamiento generador por los cambios en la posición. Se conectan dos pulsadores a los pines 32 y 25 sirviendo como el botón de pausa y el botón de "fire" respectivamente. El botón de pausa se encarga de parar la transmisión de datos del control al computador. El botón de "fire" determina la fuerza y posición del lanzamiento considerando los valores medidos por el acelerómetro.
Créditos (en esta sección deberán incluir sus nombres y al menos un correo electrónico de contacto)
Desarrolladores: Juan David Martínez, Nicolás David Rojas, Santiago Alfonso Luna.
Contacto: nicolasd.rojasc@uqvirtual.edu.co
Celular 3023340342
Docente: Jorge Iván
