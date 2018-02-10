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

资讯详情页 'http://121.14.27.27:88/wp-json/wp/v2/posts/'+id
需要是否已经关注，是否已经点赞字段，需要发布者id进行关注操作

资讯评论列表 http://121.14.27.27:88/wp-json/wp/v2/comments
需要 是否已经关注，是否已经点赞字段，评论信息应该是文本，而不是带了一些有各种标签的富文本

发布文章  http://121.14.27.27:88/wp-json/wp/v2/posts
发布内容的时候内容是上传带有标签在里面的字符串，img标签图片链接前缀有data：，发布之后获取过来的时候 data: 不见了，


需要新接口
转让页：需要转让页的接口，要求可以分页可以分类，具体需要字段请看原型图或设计图

出售网店接口：发布所需要的各种叁数，这个接口需要特别多字段～～具体需要字段请看 出售网店 原型图或设计图

店铺信息页面：集合出售网店发布的各种数据作为展示的一个页面；

店铺信息页面底部还有一个下单功能，所以还需要一个下单接口；

订单信息页面：下单之后的一个付款页面，需要显示订单信息， 另需要付款接口；

实名认证：实名认证的接口，包括支付宝绑定，银行卡绑定


	 
