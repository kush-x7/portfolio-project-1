# Animation

## Creating an animation

We Will learn to create CSS animation using `@keyframes` and the `animation` property.

- To create an animation we have to declare animation name like this `@keyframes animation-name {}`

Code example 👇

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

## Using Above Created animation

- The above created animation will start with the `opacity 0` and it will start from the `left` and come towards `right`
- To use the animation we use `animation-name: moveInLeft`
- `Duration` means how much time the animation will take to complete.
- `Delay` means the animation will start after 3 sec.
- `Iteration` count means repetition
- `Animation Timing Function ease out` means that the animation will `start faster` and `end slowly`

Code example 👇

```
  animation-name: moveInLeft;
  animation-duration: 5s;
  animation-delay: 3s;
  animation-iteration-count: 3;
  animation-timing-function: ease-out;
```

Short hand code example 👇

```
  animation: name duration timing-function delay iteration-count direction fill-mode;
```
