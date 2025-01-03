# Piedra, Papel o Tijera con Seguimiento de Manos

## Descripción del Proyecto
Este proyecto implementa un juego de **Piedra, Papel o Tijera** utilizando **Python**, **OpenCV** y **Mediapipe** para el seguimiento de manos. El objetivo principal es ofrecer una experiencia interactiva donde los usuarios pueden jugar utilizando gestos con sus manos en lugar de un teclado o ratón.

---

## Características

- **Seguimiento de Manos en Tiempo Real:** Utiliza Mediapipe para detectar las manos y sus posiciones en un flujo de video.
- **Gestos para Jugar:** Detecta los gestos de **Piedra**, **Papel** y **Tijera** basados en la configuración de los dedos.
- **Modo Individual y Multijugador:**
  - **1 Jugador:** Juega contra la IA, que selecciona aleatoriamente Piedra, Papel o Tijera.
  - **2 Jugadores:** Ambos jugadores interactúan utilizando sus gestos.
- **Interfaz Visual:** Muestra mensajes, separadores en pantalla y las decisiones de cada jugador.
- **Indicación de Ganador:** Determina el ganador según las reglas del juego.

---

## Requisitos del Sistema

- **Python 3.7 o superior**
- **Librerías Necesarias:**
  - OpenCV
  - Mediapipe
  - Imutils
- Una cámara web funcional

---

## Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/tu_usuario/piedra-papel-tijera.git
   ```

2. Navega al directorio del proyecto:
   ```bash
   cd piedra-papel-tijera
   ```

3. Instala las dependencias requeridas:
   ```bash
   pip install opencv-python mediapipe imutils
   ```

---

## Archivos del Proyecto

1. **`SeguimientoManos.py`**:
   - Contiene la clase `detectormanos`, que permite detectar manos, identificar gestos y calcular distancias entre puntos clave.

2. **`Juego.py`**:
   - Implementa la lógica del juego.
   - Detecta gestos y gestiona el flujo de juego entre el usuario y la IA o entre dos jugadores.

3. **`imagenes/`**:
   - Carpeta que contiene las imágenes utilizadas para mostrar en pantalla (por ejemplo, los gestos de Piedra, Papel, Tijera, y los resultados del juego).

---

## Cómo Jugar

1. Ejecuta el archivo principal:
   ```bash
   python Juego.py
   ```

2. **Modo 1 Jugador:**
   - Levanta tu mano frente a la cámara para seleccionar el modo de juego.
   - Usa gestos para jugar Piedra, Papel o Tijera contra la IA.

3. **Modo 2 Jugadores:**
   - Ambos jugadores colocan sus manos frente a la cámara.
   - Realizan gestos simultáneamente para competir entre sí.

4. Para reiniciar el juego, presiona la tecla `R`.
5. Para salir, presiona la tecla `Esc`.



