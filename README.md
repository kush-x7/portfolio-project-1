# Topics I have learned while making this project

👇 **_Plus, I made notes for quick revision_** 👇

## Lecture 1

![First lecture](md-images/lecture%201.png)

### 1. Basic Reset 👇

- Instead of adding font-family in universal selector, add it into a body selector.

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

<br />

### 2. Header Background + Image 👇

![example](md-images/2.png)

- **Background size cover** means covering the whole div which also includes zoom in the picture.
- **Background size contain** means it will not zoom in thepic and exact size of the image will be displayed.
- The **clip-path** property creates a clipping region where content within it is visible, and content outside it is invisible.
- Always set **image url** after the **background gradient**.

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

</br>

### **_3 You can generate more clip path from this site_** 👉 [site Link](https://bennettfeely.com/clippy/)

![example](md-images/3.png)

---

<br />

### 4 Logo 👇

![logo](md-images/4.png)

```
  <div class="logo-box">
        <img src="img/logo-white.png" alt="logo" class="logo" />
  </div>

  .header{
    position: relative;
  }

  .logo-box {
  position: absolute;
  top: 4rem;
  left: 4rem;
}

.logo {
  height: 3.5rem;
}

```

---

<br />

### 4 Centering text-box with 'POSITION + TRANSLATE) 👇

![logo](md-images/5.png)

- **Translate** will move the box on X,Y axis half of it's width and height

```
.text-box {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

---

<br/>

### 5 Animation 👇

- We use **'@keyframes animation name'** to make an animation

```
@keyframes moveInLeft {
  0% {
    opacity: 0;
    transform: translateX(-10rem);
  }
  80% {
    transform: translateX(2rem);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}


```

- The above animation means that the animation will start with the **opacity 0 and also from the left side** .
- To use the animation we use **'animation-name: moveInLeft'**
- **Duration** means how much time the animation will tak eto complete.
- **Delay** means the animation will start after 3 sec.
- **Iteration** count means repetition
- **Animation Timing Function ease out** means that the animation will start faster and end slowly

```
  animation-name: moveInLeft;
  animation-duration: 5s;
  animation-delay: 3s;
  animation-iteration-count: 3;
  animation-timing-function: ease-out;
```

- **Short hand Property** to mention all above property

```
  animation: name duration timing-function delay iteration-count direction fill-mode;
```

---
