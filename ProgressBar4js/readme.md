# 进度条组件, 只用于展示，提供进度信息的展示
元数据
```json
{
	"componentType": "ProgressBar",
	"name" : "progress1", //指定组件的名字
    "title" : "当前上传进度:${progress}/${maxProgress}", //进度上显示的提示文字 progress变量是当前进度值，
	"progress" : 20,//设置当前组件默认进度的数字0-最大进度值
	"maxProgress" : 100, //最大进度值，
	"width" : 80, //组件宽度 数字或者 null
	"height" : 20 //组件高度 数字或者 null
}
```

## 组件方法

| 方法               | 简介                 |      |
| ------------------ | -------------------- | ---- |
| getValue()         | 获取组件当前的进度值 |      |
| setValue(progress) | 设置组件当前的进度值 |      |
|                    |                      |      |


