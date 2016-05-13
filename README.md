## 学习资源

1. [W3School CSS3动画](http://www.w3school.com.cn/css3/css3_animation.asp)

## 基本概念

关键帧与关键帧之间的动画可以由软件来创建，叫做过渡帧或者中间帧。

### 动画必要条件

##关键帧、运行时间##

动画轨迹由多个关键帧组成。

在CCS3中，运行时间缺省值0（就是没有效果），如下代码，实现10秒圆形水平移动整个浏览器的宽度。

```css
.circle {
	position: absolute;
	left: 0%;
	top: 0%;
	width: 50px;
	height: 50px;
	margin: 10px;
	background-color: green;
	border-radius: 25px;

	animation-name : move;
	animation-duration : 10s;
}

@keyframes move {
	0% {
		left: 0%;
	}
	100% {
		left: 100%;
	}
}
```

其中，`animation-timing-function`作用是速度曲线用于使变化更为平滑，缺省值'ease'，速度两头快中间慢效果；

`animation-iteration-count`动画播放的次数，缺省值为1，最大值为infinite。

### 简写语法

animation: name duration timing-function delay iteration-count direction;




