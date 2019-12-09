# 提供一个组合框的面板
元数据
```json
{
	"componentType": "GroupBox",
	"name" : "userInfoGroup", //指定组件的名字
	"caption" : "工具面板",//面板正中显示的文字
	"components" : [
		{
			"componentType": "LayoutManager",
			"impl": "Flow", //Flow, Linear
			"components": [{
				"componentType": "TextEdit",
				"name": "name1", //指定组件的名字
				"caption": "注册用户名", //指定组件在需要展示标签时的名称
				"defaultValue": null //默认值
			}, {
				"componentType": "IntegerEdit",
				"name": "age1", //指定组件的名字
				"caption": "用户年龄", //指定组件在需要展示标签时的名称
				"defaultValue": null //默认值
			}]
		}
	]
}
```