# Canica — un mundo en equilibrio

Un juego de canicas para navegador, pensado para escritorio, teléfonos y tabletas. Recorre ocho niveles isométricos, encuentra el camino a la estrella y combina movimientos, saltos, giros de plataforma y desplazamientos de carril.

## Jugar

No necesita dependencias ni compilación. Sirve la carpeta desde cualquier servidor HTTP estático. Por ejemplo, con Python:

```bash
python3 -m http.server 3002
```

Luego abre <http://localhost:3002> en el navegador. También puedes abrir `index.html` directamente, aunque algunos navegadores limitan el guardado local en ese modo.

## Controles

- **Flechas**, **WASD** o los botones en pantalla: mover la canica.
- **Deslizar sobre el tablero**: mover en esa dirección; toca una fila para seleccionarla.
- **Saltar** o **Espacio**: arma un salto y luego elige una dirección. Solo permite superar un hueco de una casilla.
- **Girar** o **R**: rota el tablero.
- **Mover carril** o **Mayús**: desplaza la fila seleccionada.
- **Deshacer**: botón en pantalla o **Ctrl+Z**. **Reiniciar**: botón en pantalla o **Retroceso**.

Completa los objetivos especiales de cada nivel para avanzar. Las estrellas valoran la cantidad de movimientos. El progreso y la personalización se guardan en el almacenamiento local del navegador.

## Personalización

Elige entre seis skins —fútbol, baloncesto, tenis, luna, tierra y sol—, tres colores y forma esférica o cristalina. El sonido sintetizado se puede silenciar desde el botón musical.

## Archivos

- `index.html`: interfaz y controles accesibles.
- `styles.css`: presentación responsive.
- `game.js`: tablero, niveles, controles, renderizado Canvas y progreso.
