🔙 [Voltar para o Início](https://github.com/4L1C3-R4BB1T/estudos-sass "Voltar para o Início")

---

### 🔸 Condicionais

* **Sass**

```scss
$tema: oceano;
$primary-color: black;
$secondary-color: gray;

@if $tema == oceano {
    $primary-color: blue;
    $secondary-color: orange;
} 
@else if $tema == deserto {
    $primary-color: yellow;
    $secondary-color: purple;
}

p {
    color: $primary-color;
    background: $secondary-color;
}

div {
    $width: 600px;
    @if $width > 400px {
        width: $width;
        height: $width * 1.5;
    } 
    @else {
        width: $width;
        height: $width;
    }
}

@mixin type-1($size) {
    font-family: monospace;
    @if $size == 16 {
        font-size: 1em;
    } 
    @else if $size == 18 {
        font-size: 1.25em;
    } 
    @else if $size == 24 {
        font-size: 1.5em;
    }
}

h1 {
    @include type-1(24);
}

@mixin d($device) {
    @if $device == m {
        @media (max-width: 300px) {
            @content;
        }
    }
    @else if $device == t {
        @media (max-width: 600px) {
            @content;
        }
    }
    @else if $device == s {
        @media (max-width: 900px) {
            @content;
        }
    }
}

section {
    font-size: 1.5em;
    @include d(t) {
        font-size: 1.2em;
    }
    @include d(m) {
        font-size: 1em;
    }
}
```

* **CSS**

```css
p {
    color: blue;
    background: orange;
}

div {
    width: 600px;
    height: 900px;
}

h1 {
    font-family: monospace;
    font-size: 1.5em;
}

section {
    font-size: 1.5em;
}

@media (max-width: 600px) {
    section {
        font-size: 1.2em;
    }
}

@media (max-width: 300px) {
    section {
        font-size: 1em;
    }
}
```
