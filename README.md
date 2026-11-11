# Adiviná antes de ver

Juego para la exposición del informe estadístico sobre la **tasa de natalidad en Argentina (2000–2024)**.
El público apuesta contra el reloj y, recién después, se abre el telón y aparecen los datos reales.

Proyecto de Estadística y probabilidad, Tecnicatura Superior en Ciencia de Datos e IA.
Alumno: Damián Tejerina. Profesor: Sergio Mansilla.

## Cómo jugar

1. Escribí el nombre del jugador o equipo (se usa para el ranking).
2. Elegí la dificultad y el tiempo para votar (10, 15, 20, 30 segundos o sin tiempo).
3. Leé la pregunta en voz alta. El público vota levantando la mano.
4. Tocá la opción de la mayoría: se abre el telón y se muestra el gráfico real.

Teclas: `A`–`D` o `1`–`4` para elegir, `Enter` para seguir, `M` para silenciar.

## Niveles

| Nivel | Preguntas | Tiempo sugerido | Puntos |
|---|---|---|---|
| Fácil | 10: años, máximos, mínimos, comparaciones | 30 s | x1 |
| Medio | 10: media, mediana, moda, porcentajes, tendencias | 20 s | x1,5 |
| Difícil | 10: dispersión, cuartiles, asimetría, variación porcentual | 15 s | x2 |
| Mixto | 10 al azar de las 30 | 20 s | x1,5 |

Cada acierto da 100 puntos más 10 por cada segundo que sobraba, multiplicado por el factor del nivel.
Todas las respuestas se calculan con los datos del CSV: no hay valores escritos a mano.

## Ranking

Se guarda en el navegador (`localStorage`) de la computadora donde se juega, separado por nivel.
Si se abre en otro dispositivo o navegador, empieza vacío. Cada nivel se puede borrar desde la pantalla de ranking.

## Contenido

| Archivo | Qué es |
|---|---|
| `index.html` | Juego principal (30 preguntas, niveles, ranking, sonidos, temporizador) |
| `juegos/adivina-antes-de-ver-v2.html` | Versión 2: 5 preguntas, temporizador y sonidos |
| `juegos/adivina-antes-de-ver-v1.html` | Versión 1: primera versión |
| `juegos/mayor-o-menor.html` | Otro juego con los mismos datos |
| `datos/tasa-natalidad-deis-2000-2024.csv` | Datos originales (DEIS) |

Cada HTML es un archivo único con los datos adentro: se abre con doble clic, sin instalar nada.

## Publicarlo en GitHub Pages

En el repositorio: **Settings → Pages → Deploy from a branch → main / (root)**.
Queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Datos

Tasa de natalidad por 1.000 habitantes, Argentina y 24 jurisdicciones, 2000–2024. Fuente: DEIS (Ministerio de Salud).
