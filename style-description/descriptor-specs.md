# Descriptors

Specs for specific `style descriptors`.

## Default Behaviour

Each spec is required to have

| Field | Type | What and Why |
| :--- | :--- | :--- |
| `type` | String | ID of a [supported descriptor](#list-of-descriptor-types) |
| `values` | Array or Object | Style descriptor expected definition |

Optionally:

  1. `global` object. All the properties defined in this object, during parsing, are merged with each object found in the `values` array. This allows you to define once and apply to many.  Keep in mind that the individual value will overwrite the same property defined in `global`.

```
{
  "type": "spec-name",
  "global": {
    ... common fields or spec expected definitions
  },
  "values": [..] or {..}
}
```

## Common Fields

Each `value` object or `global` can use a handful of common fields, which Honey can use to interpret your style description better.

| Field | Value | Type |
| :--- | :--- | :--- |
| `comment` | describe the value | String |
| `group` | group this value by a group name | String | 

## List of descriptor types

1. `type: palette` / [Palette](#palette-spec)
1. `type: colour-map` / [Color Map](#color-map-spec)
1. `type: spacing` / [Spacing](#spacing)
1. `type: typography` / [Typography](#typography-spec)
1. `type: fontface` / [FontFace](#)
