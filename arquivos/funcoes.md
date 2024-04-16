🔙 [Voltar para o Início](https://github.com/4L1C3-R4BB1T/estudos-sass "Voltar para o Início")

---

### 🔸 Funções

* **Sass**

```scss
$roxo: $8844EE;

a {
    color: white;
    background: $roxo;

    &:hover {
        background: lighten($roxo, 20%);
    }
}

// Criar funções personalizadas
@function em($pixels, $contexto: 16) {
    @return ($pixels / $contexto) * 1em;
}

p {
    font-size: em(24);
}

@function grid($colunasm $total: 12) {
    @return ($colunas / $total) * 100%;
}

div {
    width: grid(2);
}
```

* **CSS**

```css
a {
    color: white;
    background: #8844EE;
}

a:hover {
    background: #c4a2f7;
}

p {
    font-size: 1.5em;
}

div {
    width: 16.66667%;
}
```
