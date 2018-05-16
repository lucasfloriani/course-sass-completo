# O que são funções (@function)

Destinam-se a criar blocos de códigos para serem executados em vários pontos de um script.

É muito parecido com @mixin, porem uma @function sempre tera um retorno.

```sass
@function calc($arg1, $arg2,...) {
  script que irá utilizar os $args;
  @return $res;
}
```

Exemplo:

```sass
@function quadrado($valor) {
  $res: $valor * $valor;
  @return $res;
}

h1 {
  font-size: quadrado(6) + px;
}

// Saída
// h1 {font-size: 36px;}
```

Exemplo com argumento default:
OBS: Parâmetros com valores default terão que estar por ultimo na função.

```sass
@function quadrado($valor, $und: px) {
  $res: $valor * $valor;
  @return $res + $und;
}
h1 {
  font-size: quadrado(6);
}
h2 {
  font-size: quadrado(2, em);
}

// Saída
// h1 {font-size: 36px;}
// h1 {font-size: 4em;}
```