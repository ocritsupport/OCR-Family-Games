# Cambios

## 1.0.0 — 21 de septiembre de 2026

Primera versión pública.

**Doce juegos**

- Cartas: Solitario (Klondike), Carta Blanca (FreeCell), Araña, La Pirámide y Parejas.
- Palabras: Palabras (tablero de 15×15 contra la máquina), Crucigrama, Sopa de letras y
  Ahorcado.
- Números y lógica: Sudoku, Buscaminas y 2048.

**Lo que no lleva**

- Sin anuncios, sin compras, sin cuentas y sin recogida de datos.
- Los doce juegos funcionan con el aparato desconectado. La única conexión es a
  `api.github.com`, para buscar actualizaciones, y se puede apagar en Ajustes.

**Accesibilidad**

- Tamaño de letra elegible dentro de la aplicación (Normal, Grande, Muy grande). Arranca
  en «Grande».
- Modo de contraste alto en blanco y negro.
- Nada pulsable por debajo de 60dp; los botones principales llevan texto además de icono.
- Se juega tocando, no arrastrando, en todos los juegos donde tiene sentido.
- Ningún juego tiene cuenta atrás.
- Las partidas a medias se recuperan solas al volver a abrir la aplicación.

**Por dentro**

- Diccionario de 635.090 palabras empaquetado como autómata determinista mínimo (DAWG),
  0,51 MB.
- El rival del juego de Palabras es el algoritmo de Appel y Jacobson: búsqueda exhaustiva
  con reglas fijas, no inteligencia artificial.
- Los crucigramas se arman con una lista aparte de 14.181 palabras corrientes, para que
  las respuestas sean palabras que conoce cualquiera.
- Requiere Android 8 o posterior. Funciona en teléfono y en tablet.

**Lo que conviene saber**

De los doce juegos, en el momento de publicar solo el **Solitario** se había probado a
fondo en un teléfono real; el resto está compilado y con la lógica cubierta por pruebas
automáticas, que no es lo mismo. Si encuentra algo raro, abra una incidencia.
