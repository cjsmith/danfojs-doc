---
description: >-
  Obtain the position of the last found occurrence of a specified value in a
  string
---

# Series.str.lastIndexOf

danfo.Series.str.lastIndexOf(str, options) \[[source](https://github.com/javascriptdata/danfojs/blob/master/src/danfojs-base/core/strings.ts#L397)]

| Parameters | Type   | Description                                                    | Default                                                |
| ---------- | ------ | -------------------------------------------------------------- | ------------------------------------------------------ |
| str        | string | the string to search for                                       | ""                                                     |
| options    | Object | **inplace**: Whether to perform the operation in-place or not. | <p>{</p><p><strong>inplace</strong>: false</p><p>}</p> |

**Returns**: Series

**Example**

{% tabs %}
{% tab title="Node" %}

```javascript
const dfd = require("danfojs-node");

let data = ["lower", "CAPITALS", "this is a sentence", "SwApCaSe"];
let sf = new dfd.Series(data);
sf.str.lastIndexOf("r").print();
```

{% endtab %}

{% tab title="Browser" %}

```

```

{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Output" %}

```
╔═══╤══════════════════════╗
║   │ 0                    ║
╟───┼──────────────────────╢
║ 0 │ 4                    ║
╟───┼──────────────────────╢
║ 1 │ -1                   ║
╟───┼──────────────────────╢
║ 2 │ -1                   ║
╟───┼──────────────────────╢
║ 3 │ -1                   ║
╚═══╧══════════════════════╝
```

{% endtab %}
{% endtabs %}
