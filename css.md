# CSS

## Grid

### Prevent Grid Item Blowout

Using `1fr` as a unit results in grid items overflowing the available grid space. This happens because `1fr` is actually treated as `minmax(auto, 1fr)`.

Prevent this "grid blowout" by using `minmax(0, 1fr)`.

```css
.grid-container {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 200px;
}
```

## Media Queries

### Prevent Sticky Hover Styles

Some touch devices emulate `:hover`, resulting in "sticky" hover styles.

This can be prevented by using `@media(hover: hover)` to check if the primary input source can hover conveniently.

```css
@media (hover: hover) {
  a:hover {
    text-decoration: underline;
  }
}
```
