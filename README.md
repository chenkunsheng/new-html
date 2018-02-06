# ios对接
每一段文字解释上面code的type属性
```
var content = {"type":"weixin_friend","title":"标题","info":"描述","img":"图片链接","id":"37"}
var data = JSON.stringify(content);
ttf.nslog(data)
```
type ：weixin_friend:微信朋友分享；  weixin_circle:微信朋友圈分享；  weibo:新浪微博分享；


```
var data = {"type":"href","id":"37"}
```
href:跳转到详情页； 


```
var data = {"type":"hrefTo","link":"/user/collection"}
```
href:跳转到对应链接；
 

```
var data = {"type":"add_post_end"}
```
add_post_end:发布资讯完成；

```
var data = {"type":"prove_end"}
```
prove_end:实名认证完成；
 


# 后台对接 
	 
