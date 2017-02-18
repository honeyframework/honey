# Spacing

### 1. `.json` structure

```
{
  "type": "spacing",
  "values": {
    ... expected definition
  }
}
```

### 2. Expected Definition

|Field|What and Why|Expected Values|Type|Required|
|:-|:-|:-|:-|:-|
|`small`|Smallest spacing, usually for menubars and shiq|*|int|No|
|`default`|The common spacing value, to be used for mostly everything.|*|int|Yes|
|`large`|Larger spacing, for what I'm not sure yet.|*|int|No|

### 3. Yields

*Remember that variable names are prepended with the respective preprocessor prefix.*

|Name / Reference|Type|Content|Dependencies|
|:-|:-|:-|:-|
|`spacing-small`|variable|value|-|
|`spacing-default`|variable|value|-|
|`spacing-large`|variable|value|-|
|`bubble-spacing-in-row`|mixin|-|-|
|`bubble-spacing-in-col`|mixin|-|-|
|`capture-spacing-in-row`|mixin|-|-|
|`capture-spacing-in-col`|mixin|-|-|
|`.scaffold`|CSS class||-|
|`.row`|CSS class|-|`.scaffold`|
|`.col`|CSS class|-|`.scaffold`|
|`.bubble-spacing-small`|CSS class|-|`.scaffold`, `.row` or `.col`|
|`.bubble-spacing-default`|CSS class|-|`.scaffold`, `.row` or `.col`|
|`.bubble-spacing-large`|CSS class|-|`.scaffold`, `.row` or `.col`|
|`.capture-spacing-small`|CSS class|-|`.scaffold`, `.row` or `.col`|
|`.capture-spacing-default`|CSS class|-|`.scaffold`, `.row` or `.col`|
|`.capture-spacing-large`|CSS class|-|`.scaffold`, `.row` or `.col`|
|`.both-ends`|CSS class|-|`.scaffold`, `.row`|
