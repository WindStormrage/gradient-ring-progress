## gradient-ring-progress 渐变环形进度条

gradient-ring-progress是js编写的渐变环形进度条插件，该插件小巧不依赖其他的库
### Demo
[gradient-ring-progress](https://progress.lap.360.cn/)
### Install
```
npm i gradient-ring-progress -S
```
### Quick Start
``` JavaScript
<div id="progress" style="height: 500px; width: 500px;"></div>
import Progress from 'gradient-ring-progress'
const progress = new Progress({
  dom: document.getElementById('progress')
})
progress.init()
```
### Options

参数 | 默认值 | 含义
---|---|---
dom | - |[必填]进度条的父级元素
color | [['rgba(238, 73, 41, 1)', 0], ['rgba(149, 236, 105, 1)', .5], ['rgba(86, 179, 255, 1)', 1]] | 颜色值[[颜色1,百分值], ...] 
type | canvas | 实现方式(canvas, svg) 现在只有canvas
value | 0.75 | 值, 0到1之间的数值
num | 300 | 分段数,越大渐变越精细
round | true | 是否圆角
duration | 3000 | 动画时长(需要大于分段数)
innerRadius | 50 | 内圆半径
outerRadius | 60 | 外圆半径
degree | 0 | 开始角度
counterclockwise | false | 是否为逆时针
bgColor | rgba(238, 239, 243, 1) | 背景环颜色,不想要可设置为透明
fontColor | rgba(58, 87, 168, 1) | 文字颜色
fontSize | 16 | 文字大小
suffix | % | 文字后缀
toFixed | 1 | 小数位

### Function

方法名 | 参数 | 含义
---|---|---
setVal | val | 修改进度条的数据
remove | - | 删除节点

### Example
![image](https://i.postimg.cc/zvjJT8c7/progress.png)
