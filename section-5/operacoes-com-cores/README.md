# Operações com cores

No Sass podemos realizar soma, subtração e multiplicação de cores nos canais red, green e blue.

OBS: Só é possível a operação em cores com o mesmo alpha (transparência).

```sass
#112233 + #223344 // Resulta em #335577
#330044 * 2 // Resulta em #660088
red - 9 // Resulta em #f60000
red + blue - 4 // Resulta em #fb00fb
rgb(100, 100, 100) + rgb(20, 30, 40) // Resulta em rgba(120, 130, 140)
rgba(100, 100, 100, 0.5) + rgba(20, 30, 40, 0.6) // Resulta em SyntaxError, alpha diferente
```

## Cores HSL

HSL (Hue, Saturation, Lightness).

Os parâmetros de core utilizados nesse sistema são tonalidade (hue, 0 à 360), saturação (saturation, 0% à 100%) e brilho (lightness, 0% à 100%). Exemplo:

```sass
h1 {
  color: hsl(120, 75%, 50%);
}
```

### Mais exemplos de cores HSL

```sass
hsl(0, 100%, 50%) // vermelho
hsl(120, 100%, 50%) // verde
hsl(120, 100%, 25%) // verde escuro
hsl(120, 100%, 75%) // verde claro
hsl(120, 75%, 75%%) // verde pastel
hsl(60, 100%, 50%%) // amarelo
hsl(120, 100%, 50%%) // verde
hsl(250, 100%, 50%%) // azul
hsl(300, 100%, 50%%) // purpura
```

## Funções para cores

darken(escurecer) e lighten(clarear)

```sass
lighten(blue, 30%) // Resulta em #9999ff
lighten(#00, 40%) // Resulta em #666666
darken(blue, 30%) // Resulta em #000066
darken(#fff, 40%) // Resulta em #999999
```

saturate (aumentar) e desaturate (diminuir)

```sass
saturate(#404040, 100%) // Resultado #800000
desaturate(#8fef8f, 40%) // Resultado #a9d5a9
```

adjust-hue - altera a tonalidade

```sass
adjust-hue(#f00, 50%) // Resultado #ffd500
adjust-hue(#00f, -50%) // Resultado #00d4ff
```

rgba(cor, alpha)

```sass
rgba(#f00, 0.5) // rgba(255, 0, 0, 0.5)
rgba(black, 0.3) // rgba(0, 0, 0, 0.3)
```