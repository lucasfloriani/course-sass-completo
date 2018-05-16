# Funções nativas do Sass

## Funções para cores RGB

* rgb($red, $blue, $green);
* rgba($red, $blue, $green, $alpha);
* red($cor);
* blue($cor);
* green($cor);
* mix($cor1, $cor2, $porcentagem);

## Funções para cores HSL

* hsl($hue, $saturation, $lighten);
* hsla($tom, $sat, $lum, $alpha);
* hue($cor);
* saturation($cor);
* lightness($cor);
* grayscale($cor);
* complement($cor);
* invert($cor);

E outras que já verificamos:

* adjust-hue
* lighten
* darken
* saturate
* desaturate

## Funções para opacidade

* alpha($cor); ou opacity($cor);
* rgba($cor, $alpha);
* opacify($cor, $val); ou fade-in($cor, $val);
* transparentize($cor, $val) ou fade-out($cor, $val);

## Funções para strings

* unquote($string);
* quote($string);
* str-length($string);
* to-upper-case($string);
* to-lower-case($string);

## Funções para números

* percentagem($num);
* round($arredonda);
* ceil($arred-proximo);
* floor($arred-anterior);
* min($numeros...);
* max($numeros...);
* random($limite);

## Funções para listas

* length($lista);
* nth($lista, $pos-item);
* set-nth($lista, $pos-item, $novo-valor);

## Funções para mapas

* map-get($mapa, $chave);
* map-merge($mapa1, $mapa2);
* map-remove($mapa, $chaves...);