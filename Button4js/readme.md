普通按钮，按钮左边可显示图标
元数据
```json
{
	"componentType": "Button",
	"name" : "okButton", //指定组件的名字
	"icon" : "suyan4j-icon-execute",//按钮图标，如果为null或空字符串不显示
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
		]
	}
}
```