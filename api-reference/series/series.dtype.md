---
description: Obtain the dtype of a series
---

# Series.dtype

> danfo.Series.dtype \[[source](https://github.com/javascriptdata/danfojs/blob/master/src/danfojs-base/core/series.ts#L19267)]

**Parameters**: None

**Returns:** String

**Example**

{% tabs %}
{% tab title="Node" %}

```javascript
const dfd = require("danfojs-node");

let data1 = [30.21091, 40.190901, 3.564, 5.0212];
let sf1 = new dfd.Series(data1);

console.log(sf1.dtype);
```

{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Output" %}

```
float32
```

{% endtab %}
{% endtabs %}
