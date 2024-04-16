🔙 [Voltar para o Início](https://github.com/4L1C3-R4BB1T/estudos-sass "Voltar para o Início")

---

### 🔸 Operadores

* **Sass**

```scss
p {
    font-size: 16px + 10;
}

h1 {
    font-size: 1em + 2;
}

$gutter: 20px;
$width: 400px;

div {
    width: $width - 2 * $gutter;
    padding: $gutter;
    height: $width / 2;
}

a {
    background: #333 + #777;
}
```

* **CSS**

```css
p {
    font-size: 26px;
}

h1 {
    font-size: 3em;
}

div {
    width: 360px;
    padding: 20px;
    height: 200px;
}

a {
    background: #aaaaaa;
}
```
