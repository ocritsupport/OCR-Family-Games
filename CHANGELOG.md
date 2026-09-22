# Cambios

## 1.0.1 — 22 de septiembre de 2026

Arreglos y una mejora salidos de probar la 1.0.0 en tablet y en teléfono.

- **En el teléfono no se leían las letras de las casillas.** En el Crucigrama, la Sopa de
  letras, el Sudoku, Palabras y Parejas, la letra salía cortada o fuera de la casilla. Al
  fijar solo el tamaño de la letra, el alto de línea seguía siendo el general de la
  aplicación, de modo que en una casilla de 25 puntos el texto ocupaba 34. En tablet, con
  las casillas grandes, no se notaba.
- **El Crucigrama daba por buenas casi todas las combinaciones** como «palabra extra»,
  porque las comprobaba contra el diccionario de 635.000 palabras, que admite rarezas como
  BOSAR, BROA o ROBS. Ahora se miden con la lista de palabras corrientes, la misma con la
  que se arman los crucigramas.
- **Se pueden arrastrar las cartas** en el Solitario, Carta Blanca, Araña y La Pirámide.
  Tocar origen y destino sigue funcionando igual: no se quita, porque para quien no tiene
  pulso para arrastrar es la única forma cómoda de jugar.
- El Crucigrama ya no carga el diccionario grande, así que abre antes.

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
