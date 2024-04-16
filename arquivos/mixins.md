🔙 [Voltar para o Início](https://github.com/4L1C3-R4BB1T/estudos-sass "Voltar para o Início")

---

### 🔸 Mixins

* **Sass**

```scss
@mixin title-large {
    font-size: 4em;
    line-height: 1;
    font-weight: bold;
    font-family: monospace;
}

h1 {
    @include title-large;
    color: blue;
}
```

* **CSS**

```css
h1 {
    font-size: 4em;
    line-height: 1;
    font-weight: bold;
    font-family: monospace;
    color: blue;
}
```

---

### 🔸 Argumentos

* **Sass**

```scss
// @mixin nome($args...) {}
@mixin separador($color: blue, $largura) {
    &::after {
        content: '';
        display: block;
        width: $largura;
        height: 4px;
        background: $color;
    }
}

h1 {
    @include separador(#84E, 100px);
}
```

* **CSS**

```css
h1::after {
    content: '';
    display: block;
    width: 100px;
    height: 4px;
    background: #84E;
}
```

---

### 🔸 @content

* **Sass**

```scss
@mixin mobile {
    @media (max-width: 600px) {
        @content;
    }
}

p {
    color: blue;
    @include mobile {
        color: pink;
    }
}
```

* **CSS**

```css
p {
    color: blue;
}

@media (max-width: 600px) {
    p {
        color: pink;
    }
}
```
