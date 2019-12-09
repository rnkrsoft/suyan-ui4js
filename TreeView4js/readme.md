# 树形视图组件,提供一个平铺或者下拉的树形结构视图
元数据
```json
{
	"name" : "city", //指定组件的名字
	"caption" : "城市",//面板正中显示的文字
	"styleType":"dropdown", //dropdown(下拉展开)或panel(面板方式)
	"datasource" : "", //支持JSON字符串或者URL
	"multiple" : false //是否是多选组件
}
```

数据源数据结构
```json
{
 	"nodes":[
 		{
 			"name":"测试用户名",
 			"value":"test-name",
 			"selected" : false,
 			"nodes" : [
	 			{
		 			"name":"曾用名",
		 			"value":"old-name",
		 			"selected" : false
	 			},{
		 			"name":"现在用名",
		 			"value":"now-name",
		 			"selected" : false
	 			}
 			]
 		},{
 			"name":"用户年龄",
 			"value":"user-age",
 			"selected" : true
 		}
 	]
}
```

提交数据
单选
```json
{
 	"data1": "user-age"
}
```
多选
```json
{
 	"data1":[
 		"test-name",
 		"user-age"
 	]
}
```