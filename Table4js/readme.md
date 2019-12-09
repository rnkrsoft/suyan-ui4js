# 表格组件，提供基本的表格表头和表格单元，以及表格关联操作的实现
元数据
```json
{
	"componentType": "Table",
	"name" : "userInfoList", //指定组件的名字
	"caption" : "用户信息列表",//面板正中显示的文字
	"columns": [
		{
			"componentType": "TextEdit",
			"name": "name1", //指定组件的名字
			"caption": "注册用户名", //指定组件在需要展示标签时的名称
			"defaultValue": null,//默认值
			"event" : {
				"onclick": [
					{ //单击事件
						"service": "com.rnkrsoft.demo.DemoService.hello1"
						"params": [
							"name1",
							"age1"
						],
						"target": {
							"type": "Component", //Component, URL, Redirect, Nil
							"component": "name1" //Component 通过全局的组件名称选中目标结果组件
						}
					}
				],
				"onmouseover": [
					{ //鼠标移入事件
						"service": "com.rnkrsoft.demo.DemoService.hello2"
						"params": [
							"name1",
							"age1"
						],
						"target": {
							"type": "URL", //Component, URL, Redirect, Nil
						}
					}
				],
				"onmouseout": [
					{ //鼠标移出事件
						"service": "com.rnkrsoft.demo.DemoService.hello3"
						"params": [
							"name1",
							"age1"
						],
						"target": {
							"type": "Redirect", //Component, URL, Redirect, Nil
						}
					}
				],
			}
		}
	]
}
```
