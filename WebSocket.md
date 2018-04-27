# WebSocket

WebSocket 是html5新增加的一种通信协议，目前流行的浏览器都支持这个协议

##  WebSocket协议简介

WebSocket协议是一种双向通信协议，它建立在TCP之上，同http一样通过TCP来传输数据，但是它和http最大的不同有两点：

1、WebSocket是一种双向通信协议，在建立连接后，WebSocket服务器和Browser/UA都能主动的向对方发送或接收数据，就像Socket一样，不同的是WebSocket是一种建立在Web基础上的一种简单模拟Socket的协议；

2.WebSocket需要通过握手连接，类似于TCP它也需要客户端和服务器端进行握手连接，连接成功后才能相互通信。

## WebSocket API简介

