# Centering Text Box Using Position + Transform

![example image](../md-images/5.png)

First center the box by mentioning `top` and `left` in `absolute positioning` then use `transform` to move the centered box `top` and `left` of `it's own 50% width and height`

```
.text-box {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```
