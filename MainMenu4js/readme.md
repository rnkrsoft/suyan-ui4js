元数据
```json
{
	"componentType": "MainMenu",
	"items": [{
		"componentType": "Button",
		"name": "btn1", //指定组件的名字
		"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
		"caption": "操作1", //指定组件在需要展示标签时的名称
		"color": "rgb(123,123,123)", //支持red，#888, rgb()
		"onclick": { //单击事件
			"service": "com.rnkrsoft.demo.DemoService.hello1"
			"params": [
				"name1",
				"age1"
			],
			"target": {
				"type": "Component", //Component, URL, Redirect, Nil
				"component": "name1" //Component 通过全局的组件名称选中目标结果组件
			}
		},
		"onmouseover": { //鼠标移入事件
			"service": "com.rnkrsoft.demo.DemoService.hello2"
			"params": [
				"name1",
				"age1"
			],
			"target": {
				"type": "URL", //Component, URL, Redirect, Nil
			}
		},
		"onmouseout": { //鼠标移出事件
			"service": "com.rnkrsoft.demo.DemoService.hello3"
			"params": [
				"name1",
				"age1"
			],
			"target": {
				"type": "Redirect", //Component, URL, Redirect, Nil
			}
		},
	}, {
		"componentType": "Separator",
		"name": "separator2", //指定组件的名字
		"width": "1", //指定组件的名字,
		"color": "rgb(123,123,123)" //支持red，#888, rgb()
	}, {
		"componentType": "Menu",
		"name": "menu3", //指定组件的名字
		"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
		"caption": "菜单3", //指定组件在需要展示标签时的名称
		"color": "rgb(123,123,123)", //支持red，#888, rgb()
		"items": [{
			"componentType": "Button",
			"name": "btn31", //指定组件的名字
			"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
			"caption": "操作31", //指定组件在需要展示标签时的名称
			"color": "rgb(123,123,123)", //支持red，#888, rgb()
			"onclick": null, //单击事件
			"onmouseover": null, //鼠标移入事件
			"onmouseout": null, //鼠标移出事件
		}, {
			"componentType": "Separator",
			"name": "separator32", //指定组件的名字
			"width": "1", //分割符的宽度,
			"color": "rgb(123,123,123)" //支持red，#888, rgb()
		}, {
			"componentType": "Menu",
			"name": "btn33", //指定组件的名字
			"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
			"caption": "菜单33", //指定组件在需要展示标签时的名称
			"color": "rgb(123,123,123)", //支持red，#888, rgb()
			"items": [{
				"componentType": "Button",
				"name": "btn331", //指定组件的名字
				"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
				"caption": "操作31", //指定组件在需要展示标签时的名称
				"color": "rgb(123,123,123)", //支持red，#888, rgb()
				"onclick": null, //单击事件
				"onmouseover":null, //鼠标移入事件
				"onmouseout":null, //鼠标移出事件
			}, {
				"componentType": "Separator",
				"name": "separator332", //指定组件的名字
				"width": "1", //分割符的宽度,
				"color": "rgb(123,123,123)" //支持red，#888, rgb()
			}, {
				"componentType": "Button",
				"name": "btn33", //指定组件的名字
				"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
				"caption": "操作333", //指定组件在需要展示标签时的名称
				"color": "rgb(123,123,123)", //支持red，#888, rgb()
				"onclick": null, //单击事件
				"onmouseover":null, //鼠标移入事件
				"onmouseout":null, //鼠标移出事件
			}]
		}]
	}]
}
```