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
var data = {"type":"hrefTo","link":"/user/collection","title":"页面头部标题"}
```
hrefTo:跳转到对应链接；
 

```
var data = {"type":"add_post_end"}
```
add_post_end:发布资讯完成；

```
var data = {"type":"prove_end"}
```
prove_end:实名认证完成；
 


# 后台对接 

### 资讯详情页

需要是否已经关注接口，需要发布者id进行关注操作

### 回答列表
是否已经点赞字段

### 回答详情页
需要是否已经关注数，关注接口，点赞数

### 回答详情页的评论列表
需要评论总条数，是否已经点赞字段，点赞是，删除评论接口，

### 竞标详情
服务商报价列表的评论接口






