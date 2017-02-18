# Color Map Spec

### 1. `.json` structure

```
{
  "type": "colour-map",
  "values": [
    {
      ... expected definition
    }
  ]
}
```

### 2. Expected Definition

| Field | What and Why | Expected Values | Type | Required |
| :--- | :--- | :--- | :--- | :--- |
| `name` | The name of colour map | * | String | Yes |
| `value` | The value of the colour map| *| String| Yes|
| `isAliased` | Allows you to set the value to either a raw colour value or to alias another definition. | true, false | Bool | No |
| `is` | Allows you to define the CSS color type of this map | `fore`, `back` | String | No |

### 3. Yields

*Remember that variable names are prepended with the respective preprocessor prefix.*

| Name / Reference | Type | Content | Dependencies |
| :--- | :--- | :--- | :--- |
| `name` | variable | value | -|
| `.name` | CSS class | `background-color` / `color` | - |
