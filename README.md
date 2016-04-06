#基于 echo 前端框架实现的图片延时加载

移动端的用户更在意网络流量的节约，如果我们总是无意义的为用户加载用户未看到的图片，会使我们的 App 增加很多无意义的流量浪费。
echo.js 很好的解决了这一问题，只有屏幕当前正在显示的图片才会下载到手机本地。

##这个示例以脚本方式为开发者实现
* 示例请使用 Apploader 查看。

##开发指南

**调用示例**

```js
echo.init({
    offset: 0, // 指定距离视窗上下左右位置图片预加载 Number|String Default: 0
    throttle: 250, // 延迟加载  Number|String	Default: 250
    unload: true,
    callback: function(element, op) {
        // console.log(element, 'has been', op + 'ed')
    }
});
```

[推荐文档](http://www.echojs.com)
[推荐文档](http://www.jq22.com/jquery-info660)