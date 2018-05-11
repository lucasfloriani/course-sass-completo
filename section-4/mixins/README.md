# Mixins

Bloco de código com sintaxe Sass, que pode ser incluido uma ou mais vezes em um arquivo Sass a ser compilado.

## Mixin sem parâmetro

```sass
// mixin sem parâmetros
@mixin colorir {
  background: black;
  color: white;
}
#main {
  font: 30px/1.4 sans-serif;
  font: {
    style: italic;
    weight: bold;
    variant: small-caps;
  }
  @include colorir // chama deste modo o mixin
}
```

## Mixin com parâmetro

```sass
// mixin com parâmetros
@mixin colorirparam($cor-bg, $cor-texto) {
  background: $cor-bg;
  color: $cor-texto;
}
#texto {
  font: 30px/1.4 sans-serif;
  font: {
    style: italic;
    weight: bold;
    variant: small-caps;
  }
  @include colorirparam(black, white);// chama deste modo o mixin com parâmetro
}
```