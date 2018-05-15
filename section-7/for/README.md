# @for

```sass
// '1 Through 4' executa de 1 até 4 (inclusive)
@for $i from 1 through 4 {
  div.item-#{$i} {
    width: 20% * $i;
  }
}

// Saída
// div.item-1 {width: 20%;}
// div.item-2 {width: 40%;}
// div.item-3 {width: 60%;}
// div.item-4 {width: 80%;}
```

```sass
// '1 to 4' executa de 1 até 4 (exclusive)
@for $i from 1 to 4 {
  div.item-#{$i} {
    width: 20% * $i;
  }
}

// Saída
// div.item-1 {width: 20%;}
// div.item-2 {width: 40%;}
// div.item-3 {width: 60%;}
```

```sass
@for $i from 1 to 4 {
  $k: 2 * $i;
  div.item-#{$k * 100} {
    width: 100px * $k;
  }
}

// Saída
// div.item-200 {width:200px;}
// div.item-400 {width:400px;}
// div.item-600 {width:600px;}
```