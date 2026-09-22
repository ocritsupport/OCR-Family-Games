# Cambios

## 1.3.0 — 22 de septiembre de 2026

**Ya están los veinticuatro juegos.** Los tres que faltaban:

- **Dibujo por números** — pintar casillas siguiendo los números de los bordes hasta que
  sale un dibujo, en 5×5 y en 10×10. Ninguno obliga a adivinar: todos se sacan razonando.
- **Mahjong** — quitar las fichas de dos en dos emparejando las iguales. Sin ideogramas
  chinos: cada ficha lleva número, símbolo y color. Todos los repartos tienen solución.
- **Dominó** — contra la máquina. La ficha se coloca sola, dándole la vuelta si hace
  falta, y arriba pone siempre qué números hay en los dos extremos.

## 1.2.0 — 22 de septiembre de 2026

- **Cuatro juegos nuevos**: Torres de Hanói (con pista, que dice siempre la mejor
  jugada), Tres Picos, Golf y Conecta 4 contra la máquina con tres niveles. Ya son
  veintiún juegos.
- **El Solitario y Carta Blanca terminan la partida solos.** Cuando las columnas ya están
  ordenadas y solo falta ir tocando para que suban las cartas, lo hacen ellos, de una
  carta en una. No se adelantan: la aplicación juega la partida entera por dentro y solo
  la termina si con eso se gana seguro; mientras quede una decisión de verdad, no toca
  nada.

## 1.1.1 — 22 de septiembre de 2026

- **Carta Blanca dice por qué no vale una jugada.** Antes, cuando una jugada no valía no
  pasaba nada: ni aviso ni sonido, y eso parece una avería más que una regla. Ahora lo
  explica con un aviso que se va solo: cuántas cartas puede mover de golpe y cuántas
  lleva, qué carta hace falta encima de cuál, o que esas cartas no van seguidas.
- **Arriba, donde ponía «Huecos», ahora pone «De golpe»**: cuántas cartas se pueden mover
  de una vez. Los huecos libres ya se ven mirando la pantalla; ese número no, y es el que
  decide la partida.
- Recordatorio que ahora sale en la ayuda: en Carta Blanca **el rey no es especial**. En
  una columna vacía cabe cualquier carta —eso es del Solitario—, y lo que impide llevar
  una escalera larga a un sitio vacío es el tope de cuántas van de golpe.

## 1.1.0 — 22 de septiembre de 2026

- **El arrastre de cartas, arreglado de raíz.** Las cartas que no se dejaban coger, las
  jugadas buenas que no se quedaban puestas por mucha puntería que se pusiera y las
  cartas duplicadas o sueltas eran todas la misma cosa: al arrastrar, el juego consultaba
  el tablero tal y como estaba al repartir y no como está ahora. Pasaba en el Solitario,
  en Carta Blanca, en la Araña y en La Pirámide.
- **Una carta que se levanta y se vuelve a dejar donde estaba se queda donde estaba.**
  Antes, apartarla dos dedos y soltarla la mandaba sola a la columna de al lado.
- **La Sopa de letras ya se puede jugar.** No se podía marcar ninguna palabra, ni
  arrastrando el dedo de la primera letra a la última ni tocando una y otra. Era el mismo
  fallo de fondo.
- **Cinco juegos nuevos**: Palabra del día (adivinar una palabra de cinco letras en seis
  intentos, la misma para todo el día), Simón dice, Casillas, Recuerda el número y
  ¿Qué falta? Los cuatro últimos son de memoria.
- En la ayuda de Carta Blanca se explica por qué a veces una carta de en medio no se deja
  coger: para llevarse varias a la vez tienen que estar ya en orden y alternando color.

## 1.0.3 — 22 de septiembre de 2026

- **Arrastrar ya no exige puntería de cirujano.** Al soltar se mira el rectángulo de la
  carta y no la punta del dedo, y solo se tienen en cuenta los sitios donde la jugada
  sería legal, de modo que se puede ser generoso sin colocar nada donde no tocaba.
  Mientras se arrastra, el sitio donde va a caer se señala con un borde.

## 1.0.2 — 22 de septiembre de 2026

- **Arreglado el arrastre de cartas**, que en la 1.0.1 hacía cosas raras: cartas
  duplicadas, cartas que desaparecían de su columna y cartas sueltas por el tapete. Al
  empezar a arrastrar, la carta se quitaba de la pantalla y con ella se destruía el
  detector del gesto, así que el arrastre se quedaba colgado a medio camino. Ahora la
  carta se queda en su sitio, transparente. Además, los sitios donde se puede soltar se
  dan de baja al dejar de existir (se notaba en La Pirámide), y un arrastre colgado se
  cancela solo en cuanto se hace una jugada.
- **El crucigrama se ve más grande**: la rueda de letras pasa de 260 a 210 puntos de alto
  y ese espacio va a las casillas, que salen bastante mayores, con la letra a juego.

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
