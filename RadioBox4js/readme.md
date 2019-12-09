# 提供一个单选组件列表
元数据
```json
{
	"name" : "sexType", //指定组件的名字
	"caption" : "性别",//面板正中显示的文字
	"styleType":"dropdown", //dropdown(下拉展开)或panel(面板方式)
	"datasource" : ""//支持JSON字符串或者URL
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