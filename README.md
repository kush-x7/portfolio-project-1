# Topics I have learned while making this project

👇 **_Plus, I made notes for quick revision_** 👇

## Lecture 1

![First lecture](md-images/lecture%201.png)

### 👉 Basic Reset

> 1. Instead of adding font-family in universal selector, add it in a body selector.

```
* {
    margin: 0;
    padding:0;
    box-sizing: border-box;
}

html{
    font-size: 62.5%
}

body {
    font-family: font name;
}
```

---

### 👉 Header Background + Image

![example](md-images/2.png)

> 1. **Background size cover** means covering the whole div which also includes zoom in the picture.
> 2. **Background size contain** means it will not zoom in th epic and exact size of the image will be displayed.
> 3. The **clip-path** property creates a clipping region where content within it is visible, and content outside it is invisible.
> 4. Always set **image url** after the **background gradient**.

```
.header {
  height: 95vh;
  background-image: linear-gradient(
      to right bottom,
      rgba(126, 213, 111, 0.8),
      rgba(126, 213, 111, 0.8)
    ),
    url(../img/hero.jpg);
  background-size: cover;
  background-position: top;
  clip-path: polygon(0 0, 100% 0, 100% 75%, 0 100%);
}
```

---

> **You can generate more clip path from this site** 👉 [site Link](https://bennettfeely.com/clippy/)

![example](md-images/3.png)
