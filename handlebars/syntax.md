# Syntax

## Identifiers

```hbs
{{! Simple }}
{{foo}}

{{! Dot-separated }}
{{foo.bar}}

{{! Segment-literal }}
{{foo['bar']}}
```

> [*Identifiers* on Handlebars Documentation]
(http://handlebarsjs.com/expressions.html#basic-blocks).

## Comments

```hbs
{{!-- I'm a comment with dashes --}}

{{! I'm a comment without dashes }}
```

> [*Comments* on Handlebars Documentation]
(http://handlebarsjs.com/#comments).

## Partials

```hbs
{{> path/to/file}}
```

> [*Partials* on Handlebars Documentation]
(http://handlebarsjs.com/partials.html).

## Conditionals

### `if`

```hbs
{{#if foo}}
  <div>
    {{bar}}
  </div>
{{/if}}
```

The `if` helper will consider as *falsy values* the following:

- `false`
- `undefined`
- `null`
- `''` (empty string)
- `0`
- `[]`

### `else`

```hbs
{{#if foo}}
  <div>
    {{bar}}
  </div>
{{else}}
  <div>
    {{baz}}
  </div>
{{/if}}
```

### `unlsess`

The `unless` helper is the inverse of the `if` helper.

```hbs
{{#unless foo}}
  <div>
    {{baz}}
  </div>
{{/unless}}
```

> [*Built-In Helpers* on Handlebars Documentation]
(http://handlebarsjs.com/builtin_helpers.html#conditionals).
