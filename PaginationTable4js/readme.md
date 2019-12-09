# 分页表格组件
元数据
```json
{
	"componentType": "PaginationTable",
	"name" : "result1", //指定组件的名字
	"caption" : "查询结果",//面板正中显示的文字
	"pageSizes" : [15, 30, 45],
	"datasource" : "",//支持JSON字符串或者URL
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
