🔙 [Voltar para o Início](https://github.com/4L1C3-R4BB1T/estudos-sass "Voltar para o Início")

---

### 🔸 Extend

* **Sass**

```scss
.erro {
    color: red;
    font-weight: bold;
}

.button-erro {
    @extend .erro;
    padding: 20px;
    border: 2px solid red;
}
```

* **CSS**

```css
.erro, .button-erro {
    color: red;
    font-weight: bold;
}

.button-erro {
    padding: 20px;
    border: 2px solid red;
}
```
