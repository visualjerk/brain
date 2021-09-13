# Google Analytics

## Adding Custom Values

1. Add a custom dimension to your property as explained [here](https://support.google.com/analytics/answer/2709829?hl=en&ref_topic=2709827#set_up_custom_dimensions).
2. Set the custom dimension in your app:

```js
ga('set', {
  dimension1: 'Custom data',
})
```
