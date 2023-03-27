---
description: Returns the number of unique values in a series
---

# Series.nUnique

> danfo.Series.nUnique() \[[source](https://github.com/javascriptdata/danfojs/blob/master/src/danfojs-base/core/series.ts#L1097)]

**Parameters**: None

**Returns:** int

**Example**

{% tabs %}
{% tab title="Node" %}

```javascript
const dfd = require("danfojs-node");

let data1 = [1, 2, 3, 4, 5, 6, 7, 8, 1, 1, 22, 8, 5, 5, 5];
let sf = new dfd.Series(data1);

console.log(sf.nUnique());
```

{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Ouptut" %}

```
9
```

{% endtab %}
{% endtabs %}
