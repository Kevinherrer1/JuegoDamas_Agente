# Juego de Damas con Inteligencia Artificial

Este proyecto es un juego de **Damas** implementado en Python, donde puedes jugar contra una Inteligencia Artificial (IA) utilizando el algoritmo **Minimax**. El tablero es de tamaño 4x4 y el juego permite que las piezas se conviertan en reinas una vez que alcanzan el final del tablero contrario.

## Requisitos

Para ejecutar este juego, debes tener instalada la siguiente tecnología:

1. **Python 3.10.6**: El código está escrito en Python, por lo que es necesario tener Python instalado.
2. **Pygame**: Usamos la biblioteca **Pygame** para la interfaz gráfica y la visualización del tablero de Damas.

### Instalación de dependencias

1. Asegúrate de tener Python3.10.6 instalado. Puedes verificarlo ejecutando el siguiente comando en la terminal:

    ```bash
    python --version
    ```

2. Instala la librería **Pygame** utilizando **pip**. Para hacerlo, ejecuta el siguiente comando en la terminal:

    ```bash
    pip install pygame
    ```

3. Si aún no tienes el archivo de imagen `corona.png` para representar las piezas reinas, descárgalo o usa una imagen propia con el nombre `corona.png` en el mismo directorio del proyecto.

## Instrucciones de uso

1. **Ejecutar el juego**: Una vez que hayas instalado las dependencias y configurado la imagen de la corona, simplemente ejecuta el archivo Python para comenzar a jugar:

    ```bash
    python juego_damas.py
    ```

2. **Interacción con el juego**:
   - El juego permite que un jugador humano juegue contra una IA.
   - Las piezas blancas (`NEGRAS`) son controladas por el jugador humano, mientras que las piezas blancas (`BLANCO`) son controladas por la IA.
   - El jugador debe mover sus piezas de acuerdo a las reglas estándar de las Damas.
   - La IA realiza su movimiento automáticamente después de cada turno del jugador.

3. **Objetivo del juego**: El objetivo es capturar todas las piezas del oponente o bloquearlas para que no puedan moverse. También puedes promover una pieza a reina al llegar a la última fila del tablero.

## Estructura del código

### Clases principales

1. **Piezas**: Representa las piezas de Damas en el tablero. Maneja la posición, el movimiento y la promoción a reina (cuando llega al final del tablero).

2. **Tablero**: Define el tablero de juego, incluyendo las casillas, las piezas y sus movimientos. Es responsable de la lógica del juego, como el movimiento de las piezas, la eliminación de piezas capturadas y la determinación del ganador.

3. **AgenteIA**: Implementa la lógica de la IA utilizando el algoritmo Minimax para calcular el mejor movimiento posible basado en la evaluación del estado del tablero.

4. **Juego**: Maneja la interfaz gráfica utilizando Pygame para mostrar el tablero y las piezas, y gestionar la interacción entre el jugador y la IA.

### Funcionalidades clave

- **Movimiento de piezas**: Las piezas se mueven por el tablero respetando las reglas de las Damas.
- **Promoción a reina**: Cuando una pieza alcanza la fila opuesta del tablero, se convierte en reina.
- **Captura de piezas**: Se pueden capturar piezas del oponente al saltar sobre ellas.
- **IA**: La IA utiliza el algoritmo Minimax para elegir el mejor movimiento en función del estado del tablero.
