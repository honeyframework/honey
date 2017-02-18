# Palette Spec

### 1. `.json` structure

```
{
  "type": "palette",
  "values": [
    {
      ... expected definition
    }
  ]
}
```

### 2. Expected Definition

|Field|What and Why|Expected Values|Type|Required|
| :- | :- | :- | :- | :- |
|`name`|The name of palette colour|*|String|Yes|
|`value`|The value of the palette colour|*|String|Yes|

### 3. Yields

*Remember that variable names are prepended with the respective preprocessor prefix.*

|Name / Reference|Type|Content|Dependencies|
|:-|:-|:-|:-|
|`name`|variable|value|-|
