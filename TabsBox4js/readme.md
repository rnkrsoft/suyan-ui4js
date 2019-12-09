# 标签化的容器
元数据
```json
{
	"componentType": "TabsBox",
	"name" : "tasks", //指定组件的名字
	"caption" : "正在运行的任务",//面板正中显示的文字
	"components": [
		{
			"componentType": "TextEdit",
			"name": "name1", //指定组件的名字
			"caption": "注册用户名", //指定组件在需要展示标签时的名称
			"defaultValue": null //默认值
		}, {
			"componentType": "IntegerEdit",
			"name": "age1", //指定组件的名字
			"caption": "用户年龄", //指定组件在需要展示标签时的名称
			"defaultValue": null //默认值
		}
	]
}
```