# 列表框，提供一维的选择组件，支持单选和多选
元数据
```json
{
	"componentType": "ComboBox",
	"name" : "sexType", //指定组件的名字
	"caption" : "性别",//面板正中显示的文字
	"style":"dropdown", //dropdown(下拉,带搜索框)、dropdownList(下拉列表，无搜索框),simple(面板方式)
	"datasource" : "",//支持JSON字符串或者URL
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
