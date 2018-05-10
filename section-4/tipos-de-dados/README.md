# Tipos de dados SassScript

* Números com ou sem unidade de medida / inteiro ou real **(por exemplo: 1.5, 10, 250px)**
* Cadeias de texto, com e sem apas **(por exemplo: "lateral", 'content', principal)**
* Cores **(por exemplo: red, #cccccc, rgba(255, 255, 0, 0.8))**
* Booleanos **(por exemplo: true, false)**
* Nulos **(por exemplo: null)**
* Listas de valores, separados por espaços ou vírgulas **(por exemplo: 1.5em 2em 0 6em ou Helvetica, Arial, sans-serif)**
* Mapas de um valor para outro **(por exemplo: (key1: value1, key2: value2))**

## Acessando dados do Mapa

``` sass
$mapa: (
  chave1: value1,
  chave2: value2,
)

#teste {
  color : map-get($mapa, chave1)
}
```

## Verificar tipo da variável

``` sass
type-of(1)
// ou
type-of("Lucas")
// ou
type-of($variavel)
// ou
type_of($variavel)
```