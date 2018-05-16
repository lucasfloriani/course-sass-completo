# @while

```sass
$cont: 1;
@while $cont < 5 {
  .item-#{$cont} {
    width: 50px * $cont;
  }
  $cont: $cont + 1;
}

// Saída
// .item-1 {width: 50px;}
// .item-2 {width: 100px;}
// .item-3 {width: 150px;}
// .item-4 {width: 200px;}
```