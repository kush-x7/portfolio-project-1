# Images Gallery

![example](md-images/../../md-images/15.png)

## Creating HTML Structure

We will create a `composition div` which will contain `3 images`

Code example 👇

```
 <div class="composition">
    <img src="img/nat-1-large.jpg" alt="Photo 1" class="composition__photo composition__photo--p1" />
    <img src="img/nat-2-large.jpg" alt="Photo 2" class="composition__photo composition__photo--p2" />
    <img src="img/nat-3-large.jpg" alt="Photo 3" class="composition__photo composition__photo--p3" />
</div>

```

## Styling

- Giving parent div `relative positioning` then arranging the images by using `absolute positioning`
- Giving `outline-offset` to images
- Then on hovering composition and checking photos `&__photo:not(:hover)` which are not hovered and scaling them down

Code example 👇

```
.composition {
position: relative;

    &__photo {
    width: 55%;
    box-shadow: 0 1.5rem 4rem rgba($color-black, 0.4);
    border-radius: 2px;
    position: absolute;
    transition: all 0.3s;
    outline-offset: 2rem;

    &--p1 {
      left: 0;
      top: -2rem;
    }

    &--p2 {
      right: 0;
      top: 2rem;
    }

    &--p3 {
      left: 20%;
      top: 10rem;
    }

    &:hover {
      outline: 1.5rem solid $color-dark-green;
      transform: scale(1.05) translateY(-0.5rem);
      box-shadow: 0 2.5rem 4rem rgba($color-black, 0.5);
      z-index: 20;
    }

}

  &:hover &__photo:not(:hover) {
  transform: scale(0.9);
  }

}
```
