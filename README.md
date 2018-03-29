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

### 资讯详情页 'http://121.14.27.27:88/wp-json/wp/v2/posts/'+id
需要是否已经关注，是否已经点赞字段，需要发布者id进行关注操作

### 资讯评论列表 http://121.14.27.27:88/wp-json/wp/v2/comments
需要 是否已经关注，是否已经点赞字段，评论信息应该是文本，而不是带了一些有各种标签的富文本

### 发布文章  http://121.14.27.27:88/wp-json/wp/v2/posts
发布内容的时候内容是上传带有标签在里面的字符串，img标签图片链接前缀有data：，发布之后获取过来的时候 data: 不见了，


## 需要新接口

### 出售网店接口：
1.网店类型原型图只有两种，api有三种，不知道第三种是什么
2.网店性质设计图是选择的，api是输入的
3.主营类目设计图是选择的，原型图是输入的（原型图没有说明哪些类目）
4.api 地区 传了个1  不知道1是什么
5.api店铺级别传了个3，我需要知道有哪些级别分别传多少
6.商标类型是tm或者r标选择，不是输入
7.保证金跟技术年费还有是否可退款

### 店铺信息页面：
集合出售网店发布的各种数据作为展示的一个页面；
店铺信息页面底部还有一个下单功能，所以还需要一个下单接口；

### 订单：
下单之后的一个付款页面，需要显示订单信息， 另需要付款接口；

### 实名认证：
实名认证的接口，包括支付宝绑定，银行卡绑定


	 
