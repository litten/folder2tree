#folder2tree

用树形节点展示文件夹结构。
Show your folder structure with tree nodes. 
### 使用 Usage:

@param {Dom} 父级dom节点               
@param {Array} 描述文件夹层级关系对象

```js
folder2tree.init(document.getElementById("ctn"), [
	{
		"img" : [
			"sprite.png",
			"bg.png"
		]
	},{
		"js": [{
			"common": [
				"jquery.js",{
					"highcharts": [{
						"modules": ["exporting.js"]
					},
					"highcharts.js"
				]}
			]
		},{
			"index": [
				"mian.js",{
					"modules": ["mod.video.js"]
				}
			]
		}]
	},{
		"css": [
			"base.css",
			"index-main.css",
			"index-video.css"
		]
	},
	"index.html",
	"favicon.ico"
]);
```

### 展示 Show:
```
├─img
│ ├─sprite.png
│ └─bg.png
├─js
│ ├─common
│ │ ├─jquery.js
│ │ └─highcharts
│ │    ├─modules
│ │    │ └─exporting.js
│ │    └─highcharts.js
│ └─index
│    ├─mian.js
│    └─modules
│       └─mod.video.js
├─css
│ ├─base.css
│ ├─index-main.css
│ └─index-video.css
├─index.html
└─favicon.ico
```

