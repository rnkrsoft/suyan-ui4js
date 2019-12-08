平铺的或者下拉展开的列表选择框
元数据
```json
{
	"metadata":{
		"name" : "data1", //指定组建的名字
		"caption" : "用户数据", //指定组件在需要展示标签时的名称
		"styleType":"dropdown", //dropdown(下拉展开)或panel(面板方式)
		"datasource" : ""//支持JSON字符串或者URL
	}
}
```
数据源数据结构
```json
{
 	"nodes":[
 		{
 			"name":"测试用户名",
 			"value":"test-name",
 			"selected" : false
 		},{
 			"name":"用户年龄",
 			"value":"user-age",
 			"selected" : true
 		}
 	]
}
```

提交数据
```json
{
 	"data1":[
 		"test-name",
 		"user-age"
 	]
}
```