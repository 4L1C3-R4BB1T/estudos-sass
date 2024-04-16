🔙 [Voltar para o Início](https://github.com/4L1C3-R4BB1T/estudos-sass "Voltar para o Início")

---

### 🔸 Nesting

* **Sass**

```scss
ul.menu {
    text-align: center;

    li {
        list-style: none;
        display: inline-block;

        a {
            padding: 20px;
            display: block;
            text-decoration: none;

            &:hover {
                opacity: 0.5;
            }
        }
    }
}
```

* **CSS**

```css
ul.menu {
    text-align: center;
}

ul.menu li {
    list-style: none;
    display: inline-block;
}

ul.menu li a {
    padding: 20px;
    display: block;
    text-decoration: none;
}

ul.menu li a:hover {
    opacity: 0.5; 
}
```
