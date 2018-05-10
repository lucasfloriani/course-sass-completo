# Importação de arquivos

Utilizado para importar outros arquivos de style dentro de outros.
Pode-se importar arquivos com extensão:

* .scss
* .sass
* .css
* url de arquivos css/sass/scss

## Sintaxe

``` sass
@import 'reset.sass';
// ou sem extensão
@import 'reset';

@import 'variaveis.scss';
// ou sem extensão
@import 'variaveis';

// ou todos juntos
@import 'reset', 'variaveis';

@import "arquivo.scss" screen;
@import url('https://fonts.googleapis.com/css?family=Roboto');
```