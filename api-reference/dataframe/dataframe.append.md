---
description: Adds new row to the end of a DataFrame
---

# DataFrame.append

danfo.DataFrame.**append**(values, index, options) \[[source](https://github.com/javascriptdata/danfojs/blob/dev/src/danfojs-base/core/frame.ts#L3130)]

| Parameters | Type                       | Description                                                                                                                                      | Default                                                 |
| ---------- | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------- |
| values     | Array, Series or DataFrame | Value to append to the DataFrame                                                                                                                 |                                                         |
| index      | Array                      | The new index value(s) to append to the Series. Must contain the same number of values as`newValues` as they map `1 - 1`.                        |                                                         |
| options    | Object                     | <p>Optional parameters</p><p><strong>inplace</strong>: Boolean indicating whether to perform the operation inplace or not. Defaults to false</p> | <p>{</p><p><strong>inplace</strong> : false</p><p>}</p> |

## **Examples**

### **Appends a new row to the end of a DataFrame**

{% tabs %}
{% tab title="Node" %}

```javascript
let data = [
  [0, 2, 4, "b"],
  [360, 180, 360, "a"],
  [2, 4, 6, "c"],
];

let df = new dfd.DataFrame(data);
df.print();

let new_df = df.append([[20, 40, 60, "d"]], [3]);
new_df.print();
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
╔═══╤═══════════════════╤═══════════════════╤═══════════════════╤═══════════════════╗
║   │ 0                 │ 1                 │ 2                 │ 3                 ║
╟───┼───────────────────┼───────────────────┼───────────────────┼───────────────────╢
║ 0 │ 0                 │ 2                 │ 4                 │ b                 ║
╟───┼───────────────────┼───────────────────┼───────────────────┼───────────────────╢
║ 1 │ 360               │ 180               │ 360               │ a                 ║
╟───┼───────────────────┼───────────────────┼───────────────────┼───────────────────╢
║ 2 │ 2                 │ 4                 │ 6                 │ c                 ║
╚═══╧═══════════════════╧═══════════════════╧═══════════════════╧═══════════════════╝


╔═══╤═══════════════════╤═══════════════════╤═══════════════════╤═══════════════════╗
║   │ 0                 │ 1                 │ 2                 │ 3                 ║
╟───┼───────────────────┼───────────────────┼───────────────────┼───────────────────╢
║ 0 │ 0                 │ 2                 │ 4                 │ b                 ║
╟───┼───────────────────┼───────────────────┼───────────────────┼───────────────────╢
║ 1 │ 360               │ 180               │ 360               │ a                 ║
╟───┼───────────────────┼───────────────────┼───────────────────┼───────────────────╢
║ 2 │ 2                 │ 4                 │ 6                 │ c                 ║
╟───┼───────────────────┼───────────────────┼───────────────────┼───────────────────╢
║ 3 │ 20                │ 40                │ 60                │ d                 ║
╚═══╧═══════════════════╧═══════════════════╧═══════════════════╧═══════════════════╝
```

{% endtab %}
{% endtabs %}

---
