# Basic Css Reset

- The best way to perform a basic reset using the `universal selector`
- `1rem = 16px`, so to make our calculation easy we divided `10/16 = 62.5%` which means now `1rem = 10px`
- Always add `font-family` in body instead of universal selector or html.

Code example 👇

```
*,
*::after,
*::before {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}

body{
    font-family: font-name;
}
```
