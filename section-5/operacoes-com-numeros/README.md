# Operações com números

```sass
20px + 40 // Resulta em 60px
20px + 6px // Resulta em 26px
20px + 6em // SyntaxError
20% + 6% // Resulta em 26%
20em + 6em - 4 // Resulta em 22em
4rem + 16 - 8rem - 2 // Resulta em 10rem
20 - 1px // Resulta em 19px
```

## Multiplicação

```sass
20px * 20px // Resulta em 400px*px (400px²)
20px * 20 // Resulta em 400px
20 * 20 // Resulta em 400
```

### Transformação de número adimensional

```sass
20 * 1% // Resulta em 20%
20 * 1px // Resulta em 20px
20 * 1em // Resulta em 20em
20 * 1rem // Resulta em 20rem
```

## Divisão

Somente é executado a divisão entre valores quando:

* Dos valores da divisão um esteja em uma varivável ou retornado por uma função
* Estiverem entre parênteses e não fizerem parte de uma lista
* Forem parte de uma expressão aritmética

```sass
$numero-1 / 2
(20px) / 6px
30px / 6px + 2px - 4px
```

OBS: Divisões com números de mesma unidade de medida resultam em valor sem unidade de medida (admensional)

```sass
(20px) / 6px // Resulta em 3.33333
```

### Exemplos de divisão

```sass
$numero: 5;

// Resulta em 20px / 6 pq não tem nenhuma das regras de divisão
20px / 6

// Resulta em 20%
(100%) / 5

// Resulta em 4px
(24px / 6)

// Resulta em 4
(24px) / 6px

// Resulta em 32px pq faz parte de uma expressão aritmética
34px - 12px / 6

// Resulta em 7px
35px / $numero

// SyntaxError, unidade de medidas diferentes resulta em erro na diminuição
34px - 12em/6
```

## Operadores relacionais e de igualdade

```sass
20 > 4 // Resulta em true
4 >= 20 // Resulta em false
20 != 4 // Resulta em true
20 == 4 // Resulta em false
tassio == 'tassio' // Resulta em true
Tassio == 'tassio' // Resulta em false
Tassio != 'tassio' // Resulta em true
```