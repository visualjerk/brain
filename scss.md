# SCSS

## Optional Mixin Arguments

Mixins can receive optional arguments, by assigning a default value:

```scss
@mixin button-variant($color, $color-bg: transparent, $color-hover: $color) {
  color: $color;
  background-color: $color-bg;

  &:hover {
    color: $color-hover;
  }
}

.button-primary {
  @include button-variant(white, darkorchid);
}

.button-secondary {
  @include button-variant(darkslategray, lightgray, black);
}
```
