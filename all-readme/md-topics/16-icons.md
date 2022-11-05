# Using Icons Font

## Downloading Icon

First head over to [linea.io](https://linea.io/) and download basic fonts. Then extract iconFont file. Now we will be needing `fonts folder` and `style.css` and add them in our css folder then link it with our mail html page.

Also change the fonts `style.css` to `font-style.css` before merging with your styles.

**Always make sure to link your css file at last, so that you won't disturb the style of the project.**

Code example 👇

```
    <link rel="stylesheet" href="css/icon-font.css" />
    <link rel="stylesheet" href="css/style.css" />

```

## Using Icon

just give that element the class name of icon and the names you can find in the references.

`i` is used for italic and here I have used for my font icon
To increase the size of our icon we can use `font-size`.

Code example 👇

```
 <i class="feature-box__icon icon-basic-world"></i>
```
