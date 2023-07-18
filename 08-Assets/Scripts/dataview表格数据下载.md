通过dataview插件，设置查询条件，查询到数据自动生成表格（csv文件），代码如下
自己把代码换成dataviewjs，并更换`<source>`查询条件，`<field1>`为查询字段即可。
```js
let source = dv.pages("<source>");
const table = source.map(p => [p.<field1>,p.<field2>,p.<field3>]);
let csvContent = "data:text/csv;charset=utf-8," + table.map(e => e.join(",")).join("\n");
var encodedUri = encodeURI(csvContent);
var link = document.createElement("a");
link.setAttribute("href", encodedUri);
link.setAttribute("download","my_data.csv");
document.body.appendChild(link);
link.click();
```
