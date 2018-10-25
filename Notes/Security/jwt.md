# JWT 

JWT 全称：Json Web Token，是一个非常轻量的规范，用于在client 和 server之间安全的传递信息

JWT 由三部分组成：

* Header
* Payload
* Signature

他们之间的关系如图：

![JWT](./../../assets/graphes/jwt.png)


## Header

描述JWT的基本信息，如类型和加密算法，用base64编码

## Payload

client和server传递信息的json, 使用base64编码，JWT标准规定了5个必填字段：

* iss: 该JWT的签发者
* sub: 该JWT所面向的用户
* aud: 接收该JWT的一方
* exp(expires): 过期时间
* iat(issued at): 签发时间

