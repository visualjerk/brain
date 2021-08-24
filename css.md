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
