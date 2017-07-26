下拉刷新
=======

前面下拉刷新使用的是阿里的touch配合transform.js实现的，觉得有点麻烦并且需要配置的项较多。今天在浏览github的时候发现了一个精简的下拉刷新插件[pulltorefresh.js](https://github.com/BoxFactura/pulltorefresh.js)

## 用法

```js

// 初始化
PullToRefresh.init({
	mainElement: 'body',
	onRefresh: function() { window.location.reload(); }
});

```

其本身也提供了很多api，具体请参考[pulltorefresh.js---API](https://github.com/BoxFactura/pulltorefresh.js#api)

这里常用的api有：

> **instructionsPullToRefresh：**    下拉是显示的文字
> **instructionsReleaseToRefresh：** 释放刷新是显示的文字 
> **instructionsRefreshing ：**      刷新时显示的文字 
> **onRefresh：**                    触发刷新时的回调函数

其他的API暂时还没研究是干嘛用的，后面补上。

## 项目中的应用

[pulltorefresh.js---Demo](http://www.boxfactura.com/pulltorefresh.js/demos/basic.html)*请在浏览器手机模式下，或在手机上预览效果*