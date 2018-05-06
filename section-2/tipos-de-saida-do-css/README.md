# Tipos de Saida do CSS

## Nested

Estilo padrão do sass para compilação, onde as chaves ficam na mesma linha que o ultimo ;
Exemplo:

```css
#!/bin/css
body{
  margin: 0;}
h1{
  font-size: 14px;}
```

## Expanded

O estilo expandido fica igual a codificação CSS normal.
Exemplo:

```css
#!/bin/css
body{
  margin: 0;
}
h1{
  font-size: 14px;
}
```

## Compact

As propriedades do arquivo ficam tudo na linha do seletor
Exemplo:

```css
#!/bin/css
body{ margin: 0;}
h1{ font-size: 14px; }
```

## Compressed

Tipo de saida que mais comprime o tamanho do arquivo
Exemplo:

```css
#!/bin/css
body{margin:0}h1{font-size:14px}
```

## Como comprimir

```sass
#!/bin/sass
sass style.scss style.css --style nested
sass style.scss style.css --style expanded
sass style.scss style.css --style compact
sass style.scss style.css --style compressed
```
