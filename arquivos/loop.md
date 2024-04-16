🔙 [Voltar para o Início](https://github.com/4L1C3-R4BB1T/estudos-sass "Voltar para o Início")

---

### 🔸 Loop

* **Sass**

```scss
@for $i from 1 through 6 {
    .item-#{$i} {
        width: 100px * $i;
    }
}

/*----------------------------------------------*/

$container: 1200;
$gutter: 20;
$colunas: 12;

@for $i from 1 through $colunas {
    $width: $container / $colunas * $i - $gutter;
    .grid-#{$i} {
        width: $width + px;
    }
}

/*----------------------------------------------*/

$i: 1;

@while $i <= 6 {
    .type-#{$i} {
        font-size: 16 * $i + px;
    }
    $i: $i + 1;
}

/*----------------------------------------------*/

$redes: facebook twitter pinterest instagram;

@each $rede in $redes {
    .#{$rede}-icon {
        background-image: url('../img/#{$rede}.png');
    }
}
```

* **CSS**

```css
.item-1 {
    width: 100px;
}

.item-2 {
    width: 200px;
}

.item-3 {
    width: 400px;
}

.item-4 {
    width: 400px;
}

.item-5 {
    width: 500px;
}

.item-6 {
    width: 600px;
}
```
