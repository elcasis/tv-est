# 📺 ¡Super Suma de Estrellas TV! ⭐ — Juego de Lógica y Sumas Inequívocas para Smart TV LG

Aplicación web interactiva en **un único archivo (`index.html`)** lista para alojar en **GitHub Pages** y abrir desde el navegador web integrado de una **Smart TV LG (webOS)** utilizando el mando **LG Magic Remote** (o en cualquier ordenador, tablet o pizarra digital).

Diseñada especialmente para **1 jugador (niños de 9 años)** a partir de los retos de lógica de suma de estrellas (como el *Puzzle 7* de referencia).

---

## 🌟 ¿Qué puede hacer el programa?

### 1. Selección Libre entre 7 Tamaños de Cuadrícula y 42 Ejercicios (`6 por tamaño`)
El jugador puede elegir en cualquier momento qué tamaño de cuadrado o rectángulo quiere resolver y cuál de sus **6 ejercicios** desea jugar:
* **`2x2` (Nivel 1 · Calentamiento):** 6 ejercicios de 2 filas × 2 columnas.
* **`3x2` (Nivel 2 · Explorador):** 6 ejercicios de 3 filas × 2 columnas.
* **`3x3` (Nivel 3 · Aventurero):** 6 ejercicios de 3 filas × 3 columnas.
* **`3x4` (Nivel 4 · Detective Estelar):** 6 ejercicios de 3 filas × 4 columnas (incluye como **Ejercicio #1** exactamente el **Puzzle 7** de la hoja original).
* **`4x4` (Nivel 5 · Maestro Lógico):** 6 ejercicios de 4 filas × 4 columnas.
* **`4x5` (Nivel 6 · Comandante Galáctico):** 6 ejercicios de 4 filas × 5 columnas.
* **`5x5` (Nivel 7 · Leyenda de las Estrellas):** 6 ejercicios de 5 filas × 5 columnas.

### 2. Regla Matemática de la "Fila Inequívoca" Garantizada en los 42 Ejercicios
* Cada uno de los **42 tableros** ha sido verificado matemáticamente para que **siempre exista una fila inicial cuyos valores solo puedan dar la suma objetivo de una única manera inequívoca**.
* Todas las demás filas y columnas **se construyen paso a paso a partir de esa fila inicial**: al elegir las casillas válidas (`✅`) y descartar las que sobran (`0`), una columna o fila que antes tenía varias combinaciones posibles pasa a tener **una única combinación posible**, permitiendo resolver todo el tablero razonando y **sin tener que adivinar nunca al azar**.
* Al completar cada ejercicio, el juego muestra en pantalla la **Cadena Lógica Inequívoca** exacta (`Fila X ➔ Columna Y ➔ ...`) que resuelve el reto.

### 3. Representación Visual Fiel a la Ficha Escolar + Ayudas para Niños de 9 Años
* **Patrón de Dado de 1 a 5 Estrellas (`⭐`):** Cada casilla muestra de 1 a 5 estrellas colocadas en la misma disposición visual de la ficha impresa para entrenar el conteo visual rápido (*subitización*).
* **Botón `🔢 Números: SÍ / NO`:** Permite mostrar u ocultar un pequeño círculo con el número (`1..5`) en la esquina de cada casilla según prefiera el niño.
* **Dos Herramientas de Deducción (como en el papel, obligatorias para ganar):**
  * **`⭐ Sumar Casilla (Sí Vale)`:** Selecciona una casilla que forma parte de la suma (`+100 puntos × racha`).
  * **`🚫 Marcar Incorrecta (No Vale · 0)`:** Marca con un **`0`** en la esquina inferior derecha las casillas que NO forman parte de la suma (`+100 puntos × racha`), exactamente igual que las anotaciones a lápiz de la ficha original.
* **Condición de Victoria Completa (`✅` + `0`):** Para ganar cada ejercicio, el niño **debe marcar tanto todas las casillas correctas (`✅`) como todas las casillas incorrectas (`0`)**. Si una fila o columna alcanza su suma objetivo pero aún tiene casillas sin descartar, su cabecera avisa en azul (`Faltan X de 0`) y solo pasa a **verde (`✅ ¡Lista!`)** cuando se han marcado también sus `0`.
* **Botón `💡 Pista: ¿Qué Fila o Columna es Inequívoca?`:** Analiza el tablero en tiempo real, ilumina en dorado la fila o columna que en ese instante solo admite **una única suma posible** y explica la suma exacta en la barra inferior.
* **Cabeceras Interactivas de Suma:** Al apuntar o pulsar sobre cualquier número de fila o columna con el mando de la TV, se ilumina toda la línea y el programa indica cuántas estrellas lleva sumadas, cuántas le faltan y cuántas combinaciones posibles quedan.

### 4. Gamificación para 1 Jugador y Guardado Automático
* **8 Mascotas Espaciales Elegibles:** `🚀`, `🦊`, `🦖`, `🦄`, `🤖`, `🐼`, `🐉`, `🦉`.
* **Multiplicador de Racha (`x1` a `x5 🔥`)** y **Calificación de 1 a 3 Estrellas (`⭐⭐⭐`)** en cada uno de los 42 ejercicios.
* **Rangos Galácticos Progresivos:** Desde *Cadete de las Estrellas* hasta *Leyenda del Universo (42/42)*.
* **Sonidos Musicales Integrados (Web Audio API):** Acordes de acierto, descarte y fanfarria de victoria sin archivos externos.
* **Guardado en `localStorage`:** Conserva las estrellas y récords en el televisor entre sesiones.

### 5. Optimización Especial para Navegador Web de TV LG
* Diseño panorámico **16:9 a pantalla completa (`100vw × 100vh`)** sin barras de desplazamiento vertical ni horizontal.
* Escalado automático del tamaño de casillas (`--cell-size`) según el nivel elegido (`2x2` hasta `5x5`) para verse grande y nítido desde el sofá.
* Sin etiquetas `<input>` de texto para evitar que se abra el teclado virtual de webOS.

---

## 🚀 Cómo subirlo a GitHub Pages y jugar en la TV LG

1. Crea un repositorio público en GitHub y sube el archivo [`index.html`](file:///c:/Users/elcas/Desktop/APP_Antigravity/Juego_Suma_Estrellas_TV/index.html) y este [`README.md`](file:///c:/Users/elcas/Desktop/APP_Antigravity/Juego_Suma_Estrellas_TV/README.md).
2. En GitHub, entra en **Settings → Pages**, selecciona la rama `main` (carpeta `/root`) y pulsa **Save**.
3. Abre el navegador web de tu **Smart TV LG** e introduce la URL generada (`https://tu-usuario.github.io/tu-repositorio/`).
