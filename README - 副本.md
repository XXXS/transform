# [Animation](https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Animations/Using_CSS_animations)

# 1. 配置动画 
## animation-delay (默认值 0 )
- 设置延时 元素加载完成到动画开始播放的时间
- 语法 :  animation-delay: time;
- js语法: object	object.style.animationDelay="2s"


## animation-direction   - 设置动画播放完后反向播放还是重新开始
- normal默认 |  reverse动画反向播放  | alternate 奇数次反向播放  | alternate-reverse 奇数次正向播放
- 语法: js	object.style.animationDirection="reverse" 

## animation-duration 设置动画播放时间

- 语法 :	object.style.animationDuration="3s"

## animation-iteration-count   设置动画重复次数
- infinte重复播放  or  具体播放次数 
    
- 语法: object.style.animationIterationCount=3


## animation-name 
 - 指定由@keyframes 描述的关键帧的名称

## animation-play-state
-  设置暂停和播放动画
-  running 播放  |  paused 暂停 
-  语法 animation-play-state: paused|running;
-   object.style.animationPlayState="paused"

##  animation-timing-function  设置动画加速度
 - linear 动画从头到尾的速度是相同的
 - linear	动画从头到尾的速度是相同的。	
 - ease	默认。动画以低速开始，然后加快，在结束前变慢
 - ease-in	动画以低速开始
 - ease-out	动画以低速结束
 - ease-in-out	动画以低速开始和结束
 - cubic-bezier(n,n,n,n) 取值是从 0 ~ 1 
## animation-fill-mode
 -  指定动画执行前后如何为目标元素应用样式
 - none	默认值。动画在动画执行之前和之后不会应用任何样式到目标元素。
 - forwards	在动画结束后（由 animation-iteration-count 决定），动画将应用该属性值。
 - backwards	动画将应用在 animation-delay 定义期间启动动画的第一次迭代的关键帧中定义的属性值。这些都是 from 关键帧中的值（当 animation-direction 为 "normal" 或 "alternate" 时）或 to 关键帧中的值（当 animation-direction 为 "reverse" 或 "alternate-reverse" 时）。
 - both	动画遵循 forwards 和 backwards 的规则。也就是说，动画会在两个方向上扩展动画属性。

 # 动画事件 
  - 动画开始播放事件  animationstart 
  - 动画播放结束事件   animationend
  - 动画重新开始播放事件   animationiteration
  