# ios对接
每一段文字解释上面code的type属性
```
var content = {"type":"weixin_friend","title":"标题","info":"描述","img":"图片链接","id":"37"}
var data = JSON.stringify(content);
console.log(data)
ttf.nslog(data)
```
type ：weixin_friend:微信朋友分享；  weixin_circle:微信朋友圈分享；  weibo:新浪微博分享；

```
var data = {"type":"href","id":"37"}
```
href:跳转到详情页； 

 # 后台对接

资讯列表：

需要字段：发布人的名字，发布的图片，阅读数；  

资讯详情：

需要接口：关注功能，收藏功能，
目前：评论列表返回数据格式错误，评论跟文章点赞接口404，评论已经登录提示需要登录，
	 普通用户发布评论提示“抱歉，您不能作为此用户创建文章”
