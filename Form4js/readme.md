创建一个窗体
元数据
```json
{
	"name": "createUserDialogbox", //指定组件的名字
	"caption": "创建新用户", //指定组件在需要展示标签时的名称
	"icon": "", //窗体显示的图标
	"menu": { //指定一个MainMenu组件
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
	},
	"clientHeight": 600, //窗体客户区高度
	"clientWidth": 500, //窗体客户区宽度
	"visible": true, //用于设定此窗体是否被显示
	"titleBar": [{
		"componentType": "Button",
		"icon": "suyan4j-icon-close",
		"hint": "关闭窗口",
		"type": "close", //close（关闭）, min （最小化）, max （最大化）, help（帮助）, null(自定义)
		"onclick": "", //当type为null时有效，自定义单击事件
		"onmouseover"： null, //自定义单击事件，鼠标移入事件
		"onmouseout"： null, //自定义单击事件，鼠标移出事件
	}, {
		"componentType": "Button",
		"icon": "suyan4j-icon-min",
		"hint": "最小化窗口",
		"type": "min", //close（关闭）, min （最小化）, max （最大化）, help（帮助）, null(自定义)
		"onclick": "", //当type为null时有效，自定义单击事件
		"onmouseover"： null, //自定义单击事件，鼠标移入事件
		"onmouseout"： null, //自定义单击事件，鼠标移出事件
	}],
	"components": [ //窗口中的组件
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
		}, {
			"componentType": "ToolBar",
			"name": "mainToolBar", //指定组件的名字
			"caption": "主工具栏", //指定组件在需要展示标签时的名称
			"autoSize": true, //工具栏是否自动调整大小容纳
			"components": [ //放入对应组件的元信息定义
				{
					"componentType": "Button",
					"name": "queryButton", //指定组件的名字
					"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
					"caption": "查询", //指定组件在需要展示标签时的名称
					"onclick": null, //单击事件
					"onmouseover":null, //鼠标移入事件
					"onmouseout":null, //鼠标移出事件
				}, {
					"componentType": "Separator",
					"width": "1", //指定组件的名字,
					"color": "rgb(123,123,123)" //支持red，#888, rgb()
				}, {
					"componentType": "Button",
					"name": "resetButton", //指定组件的名字
					"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
					"caption": "重置", //指定组件在需要展示标签时的名称
					"onclick": null, //单击事件
					"onmouseover"： null, //鼠标移入事件
					"onmouseout"： null, //鼠标移出事件
				}
			]
		}, {
			"componentType": "ToolBar",
			"name": "toolBar1", //指定组件的名字
			"caption": "常用工具栏", //指定组件在需要展示标签时的名称
			"autoSize": true, //工具栏是否自动调整大小容纳
			"components": [ //放入对应组件的元信息定义
				{
					"componentType": "Button",
					"name": "okButton", //指定组件的名字
					"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
					"caption": "新建", //指定组件在需要展示标签时的名称
					"onclick": null, //单击事件
					"onmouseover"： null, //鼠标移入事件
					"onmouseout"： null, //鼠标移出事件
				},
				{
					"componentType": "BitBtn",
					"name": "okButton", //指定组件的名字
					"image": "/statics/images/execute_btn.png" //指定按钮的图片
					"borderWidth": "1", //边框线宽度
					"borderColor": "red", //边框颜色
					"borderStyle": "solid", //边框样式，支持 solid 实线，dashed 虚线,dotted 点状线
					"onclick": null, //单击事件
					"onmouseover"： null, //鼠标移入事件
					"onmouseout"： null, //鼠标移出事件
				},
				{
					"componentType": "Separator",
					"width": "1", //指定组件的名字,
					"color": "rgb(123,123,123)" //支持red，#888, rgb()
				}
			]
		}, {
			"componentType": "PaginationTable",
			"name": "queryResultTable", //指定组件的名字
			"caption": "查询结果表格", //指定组件在需要展示标签时的名称
			"items": [{
				"componentType": "TextEdit",
				"name": "name1", //指定组件的名字
				"caption": "注册用户名", //指定组件在需要展示标签时的名称
				"defaultValue": null //默认值
			}, {
				"componentType": "IntegerEdit",
				"name": "age1", //指定组件的名字
				"caption": "用户年龄", //指定组件在需要展示标签时的名称
				"defaultValue": null //默认值
			}],
			"operateMenu": { //操作按钮
				"componentType": "PopupMenu",
				"items": [{
					"componentType": "Button",
					"name": "btn1", //指定组件的名字
					"icon": "suyan4j-icon-execute", //按钮图标，如果为null或空字符串不显示
					"caption": "操作1", //指定组件在需要展示标签时的名称
					"color": "rgb(123,123,123)", //支持red，#888, rgb()
					"onclick": {
						"params": [
							"name1",
							"age1"
						],
						"target": {
							"type": "Component", //Component, URL, Redirect, Nil
							"component": "name1" //Component 通过全局的组件名称选中目标结果组件
						}
					}, //单击事件
					"onmouseover"： null, //鼠标移入事件
					"onmouseout"： null, //鼠标移出事件
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
						"onmouseover"： null, //鼠标移入事件
						"onmouseout"： null, //鼠标移出事件
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
							"onmouseover"： null, //鼠标移入事件
							"onmouseout"： null, //鼠标移出事件
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
							"onmouseover"： null, //鼠标移入事件
							"onmouseout"： null, //鼠标移出事件
						}]
					}]
				}]
			}
		}
	]
}
```