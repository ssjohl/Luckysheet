# FAQ

## What is the difference between data and celldata in luckysheetfile?

**<span style="font-size:20px;">A</span>**: Use one-dimensional array format [celldata](https://mengshukeji.github.io/LuckysheetDocs/guide/data.html), after the initialization is completed, the data converted into a two-dimensional array format is used for storage and update, and celldata is no longer used.

If you need to take out data as initial data, you need to execute `luckysheet.getGridData(data)` to convert it to celldata data.
Among them, the celldata in `{ r, c, v }` format is converted to a two-dimensional array using `luckysheet.buildGridData(luckysheetfile)`, and the input parameter is the table data object `luckysheetfile`

Summarized as follows:
```js
// data => celldata two-dimensional array data is converted into {r, c, v} format one-dimensional array, the input parameter is two-dimensional data
luckysheet.getGridData(data)

// celldata => data The two-dimensional array required to generate the table, the input parameter is the table data object file
luckysheet.buildGridData(luckysheetfile)
```

------------
## What are the cell types?

**<span style="font-size:20px;">A</span>**: Refer to [Cell Format List](https://mengshukeji.github.io/LuckysheetDocs/guide/format.html), with examples of available cell formats

------------