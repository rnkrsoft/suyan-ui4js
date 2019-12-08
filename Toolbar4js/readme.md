工具栏，可放入按钮和分割线
元数据
```json
{
	"name" : "name1", //指定组件的名字
	"caption" : "注册用户名", //指定组件在需要展示标签时的名称
	"autoSize" : true,//工具栏是否自动调整大小容纳
	
	"components" : [ //放入对应组件的元信息定义
		{
			"componentType" : "Button",
			"name" : "okButton", //指定组件的名字
			"icon" : "suyan4j-icon-execute",//按钮图标，如果为null或空字符串不显示
			"onclick" : null,//单击事件
			"onmouseover" null,//鼠标移入事件
			"onmouseout" null,//鼠标移出事件
		},
		{
			"componentType" : "Button",
			"name" : "okButton", //指定组件的名字
			"image" : "/statics/images/execute_btn.png"//指定按钮的图片
			"borderWidth" : "1", //边框线宽度
			"borderColor" : "red",//边框颜色
			"borderStyle" : "solid",//边框样式，支持 solid 实线，dashed 虚线,dotted 点状线
			"onclick" : null,//单击事件
			"onmouseover" null,//鼠标移入事件
			"onmouseout" null,//鼠标移出事件
		},
		{
			"componentType" : "Separator",
			"width" : "1", //指定组件的名字,
			"color" : "rgb(123,123,123)"//支持red，#888, rgb()
		}
	]
}
```