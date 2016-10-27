控制台：document.documentElement.clientWidth = 物理像素 / 缩放比例

使用 viewport meta 标签在手机浏览器上控制布局:
<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1" />
device-width：设备宽度  initial-scale:初始的缩放  maximum-scale：最大的值的缩放

隐藏苹果浏览器的工具栏和菜单栏。 全屏显示
:
<meta name="apple-mobile-web-app-capable" content="yes" />


设置Web App的状态栏（屏幕顶部栏）的样式
:
<meta name="apple-mobile-web-app-status-bar-style" content="blank" />



实际浏览器的布局宽度：
(1) 如果没有设置viewport width=device-width; 此时布局宽度就是980px;(浏览器统一缩放的)；
		
(2) 如果设置了，布局宽度就是 ，设备的物理像素/window.devicePixelRatio 。 
    直接通过chrome 手机浏览器工具查实际浏览器布局宽度


@media screen and (orientation:landscape)横屏

@media screen and (orientation:portrait)竖屏

@media only screen and (max-width:320px ) 只适合于浏览器

@media all and (min-width:1024px)适用于所有设备包括打印机
