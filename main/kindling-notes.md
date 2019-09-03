# Kindling Notes

Some notes & thoughts about certain kindling features are found here.

### General

- Mixins should get namespaces
- ALL Context maps are located in `web/src/scss/settings/contexts`

### Form Elements

`\compass\layout\form\grid-columns\apply()`:

```scss
.fields {
    @include \compass\layout\form\grid-columns\apply();

    > * {
        &:last-child {
            &:nth-child(odd) {
                @include \kindling\breakpoint\media-query('large') {
                    grid-column-end: span 2;
                }
            }
        }
    }
}
```

NOTE: `> *` selects all direct children
