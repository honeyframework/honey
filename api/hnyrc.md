# `.hnyrc` Configuration

In the root of your UI repo, add a `.hnyrc` file. This will contain your configuration for **honey**.

#### Options

|Option|Type|What and Why|Expected Values|
|:-|:-|:-|:-|
|`name`|String|The name of your user interface, if any.|*|
|`input`|String|Define the path to your style descriptors. This allows **honey** to know from where to load your `.json` descriptors.|*dir path*|
|`preprocessor`|String|Define which CSS preprocessor you want to build for.|`sass`,`less`,`stylus`|
|`comb`|Object|Config options for **honey's** comb module.|[go to definition](#comb)|
|`dippers`|Array|Define the **dippers** you want to use, and any associated config.|[go to definition](#dippers)|

## Expected Values

#### `comb`

    "comb": {
      ... expected values
    }

|Option|Type|What and Why|Expected Values|
|:-|:-|:-|:-|
|`output`|String|The path in your repo where **honey** will put the built files.|*dir path*|
|`guideName`|String|The name of the file|*|

#### `dippers`

    "dippers": [
      {
        ... expected values
      }
    ]

|Option|Type|What and Why|Expected Values|
|:-|:-|:-|:-|
|`name`|String|The name of the **honey dipper** you want to use. If a dipper's name is `honey-dipper-example`, only put `example` here.|*|
|`output`|String|The path in your repo where this dipper will put it's respective build files.|*dir path*|
