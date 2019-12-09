# 文件盒组件，提供上传，查看，浏览一个或者多个文件的组件，如果是文件则展示为预览图和相册
元数据
```json
{
	"name" : "sexType", //指定组件的名字
	"caption" : "性别",//面板正中显示的文字
	"style":"dropdown", //dropdown（下拉展开）,simple(简单的展开)
	"datasource" : "",//支持提交数据作为数据源
	"multiple" : false //是否是多选组件
}
```

提交数据
单选
```json
{
 	"files1": "http://localhost/demo2/demo2.jpg"
}
```
多选
```json
{
 	"files1":[
 		"http://localhost/demo1/demo1.doc",
 		"http://localhost/demo2/demo2.jpg"
 	]
}
```
