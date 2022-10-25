---
<br/>
---

<br />

### 6 Button + Animation 👇

![logo](md-images/6.png)

- First create an anchor element with the class name btn

```
<a href="#" class="btn btn-white btn-animated">Discover our tours</a>
```

- Then style the anchor tag

```
.btn:link,
.btn:visited {
  text-decoration: none;
  text-transform: uppercase;
  padding: 1.5rem 4rem;
  display: inline-block;  -> Now it will behave as text
  border-radius: 10rem;

  transition: all 0.2s;
  position: relative;
}

.btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}

.btn:active {
  transform: translateY(-1px);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
```

- Above we have use transition which means it will take 0.2s while transforming.
- On hovering we will create bigger box shadow.
- On click we will make the shadow small.

```
.btn-white {
  background-color: var(--white);
  color: var(--grey);
}

.btn::after {
  content: "";
  display: inline-block;
  height: 100%;
  width: 100%;
  border-radius: 10rem;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;

  transition: all 0.4s;
}

.btn-white:after {
  background-color: var(--white);
}
```

- **AFTER** will create a content just after button with 100% height and width.
- To take the exact area we have used absolute positioning and z-index too.

```
.btn:hover::after {
  transform: scaleX(1.4) scaleY(1.6);
  opacity: 0;
}
```

- This will scale the **AFTER** box and just after zoom in the opacity will become 0.

```

.btn-animated {
  animation: moveInUp 0.5s ease-out 0.75s;
  animation-fill-mode: backwards;
}
```

- If we don't use animation-fill-mode backwards then the button will show in the starting and after 0.75s it will apply animation.
- So backwards help us to assign the animation before the delay.
