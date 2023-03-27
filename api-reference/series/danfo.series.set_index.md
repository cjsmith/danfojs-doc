---
description: Assign new Index to Series
---

# danfo.Series.setIndex

> danfo.series.**setIndex\(**kwargs**\)** \[[source](https://github.com/javascriptdata/danfojs/blob/master/src/danfojs-base/core/series.ts#L9584)\]

| Parameters | Type      | Description                                                                                                                   | Default |
| :--------- | :-------- | :---------------------------------------------------------------------------------------------------------------------------- | :------ |
| kwargs     | Object {} | The object contains the key **index** and assigned an array value of equal length to the Series. format {"index": \[Array\] } |         |

**Example**

```javascript
const dfd = require("danfojs");

let data = [
  { alpha: "A", count: 1 },
  { alpha: "B", count: 2 },
  { alpha: "C", count: 3 },
];
let df = new dfd.Series(data);
let df_new = df.set_index({ index: ["one", "two", "three"] });
df_new.print();
```

**OUTPUT**

![](../../.gitbook/assets/series.reset_index.png)

```javascript
const dfd = require("danfojs");

let data = ["Humans", "Life", "Meaning", "Fact", "Truth"];
let df = new dfd.Series(data);
let df_new = df.set_index({ index: ["H", "L", "M", "F", "T"] });
df_new.print();
```

**OUTPUT**

![](../../.gitbook/assets/series_reset_index2.png)
