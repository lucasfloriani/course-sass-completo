# Diretivas de controle

O SassScript suporta diretivas de controle e expressões básicas para incluir estilos somente sob algumas condições ou incluindo o mesmo estilo várias vezes com variações

As diretivas de controle são um recurso avançado e são incomuns no dia-a-dia. Elas existem principalmente para uso em mixins.

As diretivas de controle previstas no Sass são:

* @if
* @else
* @else if
* @for
* @each
* @while

## Estrutura das diretivas

```sass
@diretiva expressão {
  // script
}
```

### @if

```sass
@if (expressão) {
  // script
}
```

## @else

```sass
@if (expressão) {
  // script 0
} @else {
  // script 1
}
```

## @else if

```sass
@if (expressão) {
  // script 0
} @else if (expressão) {
  // script 1
} @else if (expressão) {
  // script 2
} @else {
  // script 3
}
```

```sass
@if ($cor == red) {
  // script 0
} @else if ($tamanho > 10) {
  // script 1
} @else if ($nome != 'tema-1') {
  // script 2
} @else {
  // script 3
}
```