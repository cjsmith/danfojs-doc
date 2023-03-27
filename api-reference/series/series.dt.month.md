---
description: Obtain the month in a date time series
---

# Series.dt.month

> danfo.Series.dt.**month**() \[[source](https://github.com/javascriptdata/danfojs/blob/master/src/danfojs-base/core/datetime.ts#L62)]

**Parameters**: None

**Returns:** Series (int elements)

**Examples**

{% tabs %}
{% tab title="Node" %}

```javascript
const dfd = require("danfojs-node");

let data = new dfd.dateRange({
  start: "2016-7-31",
  end: "2016-12-08",
  freq: "M",
});
let sf = new dfd.Series(data);

sf.dt.month().print();
```

{% endtab %}

{% tab title="Browser" %}

```

```

{% endtab %}
{% endtabs %}

```
╔═══╤════╗
║ 0 │ 6  ║
╟───┼────╢
║ 1 │ 7  ║
╟───┼────╢
║ 2 │ 9  ║
╟───┼────╢
║ 3 │ 9  ║
╟───┼────╢
║ 4 │ 11 ║
╟───┼────╢
║ 5 │ 11 ║
╚═══╧════╝
```
