# Typography Spec

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

| Field | What and Why | Expected Values | Type | Required |
| :--- | :--- | :--- | :--- | :--- |
| `element` | The element to which to apply the typography definition | HTML5 type element | String | Yes |
| `size` | The font size | int | String | Yes |
| `style` | The font style | `reg`, `bold`, `semibold`, `light` | String | Yes |

### 3. Yields

*Remember that variable names are prepended with the respective preprocessor prefix.*

| Name / Reference | Type | Content | Dependencies |
| :--- | :--- | :--- | :--- | 
