# `tabindex`

## Positive value

A positive number defines an explicit navigation order —*usually a bad idea.*

```html
<span tabindex="1">
  Foobar
</span>
```

## Zero

A value of zero allows the element to receive keyboard focus, and places it
in the logical navigation flow.

```html
<span tabindex="0">
  Foobar
</span>
```

## Negative value

A negative value allows the element to receive focus, but not via
keyboard navigation.

```html
<span tabindex="-1">
  Foobar
</span>
```

> [`tabindex` on W3C]
(https://www.w3.org/TR/html5/editing.html#attr-tabindex)
