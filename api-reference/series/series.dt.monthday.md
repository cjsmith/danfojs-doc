---
description: Obtain the day of the month
---

# Series.dt.dayOfMonth

> danfo.Series.dt.dayOfMonth() \[[source](https://github.com/javascriptdata/danfojs/blob/master/src/danfojs-base/core/datetime.ts#L170)]

**Parameters:** None

**Returns**: Series (Int elements)

**Examples**

{% tabs %}
{% tab title="Node" %}

```javascript
const dfd = require("danfojs-node");

let data = new dfd.dateRange({ start: "2000-01-01", period: 4, freq: "D" });
let sf = new dfd.Series(data);
//print series
sf.print();
//print monthdays
sf.dt.dayOfMonth().print();
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
║ 0 │ 1/1/2000, 1:00:00 AM ║
╟───┼──────────────────────╢
║ 1 │ 1/2/2000, 1:00:00 AM ║
╟───┼──────────────────────╢
║ 2 │ 1/3/2000, 1:00:00 AM ║
╚═══╧══════════════════════╝

╔═══╤═══╗
║ 0 │ 1 ║
╟───┼───╢
║ 1 │ 2 ║
╟───┼───╢
║ 2 │ 3 ║
╚═══╧═══╝
```

{% endtab %}
{% endtabs %}
