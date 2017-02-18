# Fonts Spec

### 1. `.json` structure

```
{
  "type": "font",
  "values": [
    {
      ... expected definition
    }
  ]
}
```

### 2. Expected Definition

|Field|What and Why|Expected Values|Type|Required|
|:-|:-|:-|:-|:-|
|`path`|This is the path to the font file's containing folder from the user's repo (so excluding the filename). This is used to generate the url used by CSS to locate the font.|*|String|Yes|
|`fontType`|The type of the font.|`fontface`|String|Yes|
|`name`|The name of the font|*|String|Yes|
|`filename`|The actual name of the font file in the user's file system.|*|String|Yes|
|`style`|The CSS class generate containing the font spec.|`reg`, `bold`, `semibold`, `light`|String|No|

### 3. Yields

*Remember that variable names are prepended with the respective preprocessor prefix.*

|Name / Reference|Type|Content|Dependencies|
|:-|:-|:-|:-|
|`font-[style]`|variable|I don't think I really need this|-|
|`.font-[style]`|CSS class|The styling to apply the relevant `font-family`|-|
