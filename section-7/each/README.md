# @each

Itera listas recebendo o valor da iteração na variavel

```sass
@each $icon in insta, face, youtube {
  .icon-#{$icon} {
    background-image: url(img/#{$icon}.png);
  }
}

// Saída
// icone-insta {background-image: url(img/insta.png);}
// icone-face {background-image: url(img/face.png);}
// icone-youtube {background-image: url(img/youtube.png);}
```

```sass
$redes-sociais: (insta, face, youtube)
@each $icon in $redes-sociais {
  .icon-#{$icon} {
    background-image: url(img/#{$icon}.png);
  }
}

// Saída
// icone-insta {background-image: url(img/insta.png);}
// icone-face {background-image: url(img/face.png);}
// icone-youtube {background-image: url(img/youtube.png);}
```