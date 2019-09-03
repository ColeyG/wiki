# Kindling Notes

Some notes & thoughts about certain kindling features are found here.

## Notes

### General

- Mixins should get namespaces
- ALL Context maps are located in `web/src/scss/settings/contexts`
- Media Queries should go _after_ styles

### Passing Values

Instead of chaining media queries, we should pass values to a mixin via a map like the following:

```scss
@include \kindling\property\apply(
  "width",
  (
    "small": 100%,
    "medium": \kindling\grid\column-width-calc(10),
    "large": \kindling\grid\column-width-calc(8),
  )
);
```

### Form Elements

`\compass\layout\form\grid-columns\apply()`:

```scss
.fields {
  @include \compass\layout\form\grid-columns\apply();

  > * {
    &:last-child {
      &:nth-child(odd) {
        @include \kindling\breakpoint\media-query("large") {
          grid-column-end: span 2;
        }
      }
    }
  }
}
```

NOTE: `> *` selects all direct children

### Fixing Linting for Values

```scss
@include \kindling\grid\column(
  $responsive-sizes: (
    "small": \kindling\grid\column-width-calc(12),
    "large": \kindling\grid\column-width-calc(5),
    "xlarge": \kindling\grid\column-width-calc(4),
  )
);
```
