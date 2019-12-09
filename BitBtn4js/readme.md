图形按钮，按钮显示为一个指定的图片
元数据
```json
{
	"componentType": "BitBtn",
	"name" : "okButton", //指定组件的名字
	"image" : "/statics/images/execute_btn.png"//指定按钮的图片
	"borderWidth" : "1", //边框线宽度
	"borderColor" : "red",//边框颜色
	"borderStyle" : "solid",//边框样式，支持 solid 实线，dashed 虚线,dotted 点状线
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