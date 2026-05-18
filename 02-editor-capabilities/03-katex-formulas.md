# KaTeX Formulas

Usa esta pagina para validar render de formulas, helpers visuales y roundtrip limpio entre rich text y Markdown.

## Inline

- Energia: $E = mc^2$
- Tiempo estimado: $t = \frac{d}{v}$
- Error medio: $\mu = \frac{1}{n}\sum_{i=1}^{n} x_i$

## Bloque principal

$$
f(x) = \int_{-\infty}^{\infty} e^{-x^2}\,dx
$$

## Sistema de ecuaciones

$$
\begin{aligned}
2x + y &= 11 \\
x - y &= 1
\end{aligned}
$$

## Matriz

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
0 & 0 & 1
\end{bmatrix}
$$

## Formula aplicada a documentacion

$$
coverage = \frac{documented\ requirements}{total\ requirements} \times 100
$$

| Zona | Que probar |
| --- | --- |
| Formula inline | edicion rapida dentro de texto |
| Formula en bloque | helper visual y render |
| Matriz | estructuras menos triviales |

> [!IMPORTANT]
> Si hay tooling `Pro` para KaTeX, esta pagina deberia ser una buena zona de humo para aceleradores de insercion y correccion.
