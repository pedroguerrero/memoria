# Juego de Memoria

Juego de cartas de memoria en un solo archivo HTML — sin dependencias, sin build, sin servidor. Abre `index.html` en cualquier navegador y juega.

## Cómo jugar

1. Elige el nivel de dificultad en el selector.
2. Haz clic en dos cartas para voltearlas.
3. Si las cartas coinciden, quedan descubiertas; si no, se vuelven a voltear.
4. Completa todos los pares con el menor número de intentos posible.

## Niveles

| Nivel   | Pares | Columnas (desktop) | Columnas (móvil ≤ 540 px) |
|---------|-------|--------------------|---------------------------|
| Fácil   | 8     | 4                  | 4                         |
| Normal  | 10    | 5                  | 4                         |
| Difícil | 15    | 6                  | 5                         |

## Características

- 30 emojis distintos mezclados aleatoriamente en cada partida.
- Animación de volteo 3D con CSS (`rotateY`).
- Animación de sacudida al fallar un par.
- Contador de intentos y pares encontrados en tiempo real.
- Mensaje de victoria con frases aleatorias al completar el tablero.
- Compatible con navegadores móviles: sin delay de toque, sin selección accidental de texto, sin menú contextual al mantener presionado.
- Diseño responsivo: en pantallas ≤ 540 px Fácil/Normal usan 4 columnas y Difícil usa 5 (6 filas en vez de 8, menos scroll).
- Fuente [Roboto](https://fonts.google.com/specimen/Roboto) via Google Fonts.

## Estructura

```
memoria/
└── index.html   # HTML + CSS + JS en un único archivo
```

## Uso

```bash
# Opción 1 — abrir directamente
open index.html

# Opción 2 — servidor local rápido (evita restricciones de file://)
npx serve .
# o
python3 -m http.server
```
