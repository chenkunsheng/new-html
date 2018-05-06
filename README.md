# ios对接
每一段文字解释上面code的type属性
```
var content = {"type":"weixin_friend","title":"标题","info":"描述","img":"图片链接","id":"37","link":"/user/collection"}
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
var data = {"type":"add_answer_end"}
```
add_answer_end:发布问答完成；



```
var data = {"type":"add_classroom_end"}
```
add_classroom_end:发布课堂完成；



```
var data = {"type":"add_wangdian_end"}
```
add_wangdian_end:发布网店完成；



```
var data = {"type":"add_bidding_end"}
```
add_bidding_end:发布竞标完成；


```
var data = {"type":"add_recruit_end"}
```
add_recruit_end:发布招聘完成；



```
var data = {"type":"prove_end"}
```
prove_end:实名认证完成；

 



# 后台对接 


### 竞标详情
服务商报价列表的评论接口

### 我的钱吧
我的余额，钱包明细，钱吧充值，钱包提现，

### 我的订单列表 

卖家跟买家 mjorderlist.php  orderlist.php

订单返回数据需要有状态判断的(是否请求成功)

需要订单编号字段

需要订单状态字段(下单未付款，已下单，部分支付，交易完成，订单已取消的判断)

### 我的订单列表 
订单可分全额付款跟部分付款



## 系统设置

### 账号与安全
账号id，绑定手机，绑定微信，修改登录密码，设置支付密码

### 隐私设置
不给他看动态，不看他动态，仅好友可评论，仅好友可发消息


## 需要用户头像的接口
资讯详情，资讯详情的用户评论，课堂列表，课堂详情，问答详情，问答详情的回答，



# 前端未完成任务

 ### 我的钱包
 
 ### 网店详情
 








  







