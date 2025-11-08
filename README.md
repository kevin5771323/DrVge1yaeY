# 前言

欢迎来到我们的"基于微信小程序的外卖点餐系统设计与实现SSM"项目。本项目旨在为用户提供便捷、高效、安全的点餐体验。通过微信小程序，用户可以轻松浏览菜单、下单支付，商家可以高效管理订单，提升运营效率。

# 内容介绍

本项目主要包括以下功能模块：用户模块、菜单模块、订单模块、支付模块。用户模块负责用户注册、登录、个人信息管理等功能；菜单模块负责菜品展示、分类、搜索等功能；订单模块负责订单创建、支付、状态追踪等功能；支付模块负责与微信支付接口对接，实现安全可靠的支付功能。

# 技术介绍

## 语言：Java
## 使用框架：Spring、Springmvc、MyBatis，微信小程序
## 前端技术：JS、Vue、CSS3，Uniapp
## 开发工具：IDEA/Eclipse，Uniapp
## 数据库：MySQL 5.7/8.0
## 数据库管理工具：phpstudy/Navicat
## JDK版本：jdk1.8
## Maven：apache-maven 3.8.1-bin
## 前端环境：Node.Js 12\14\16

# 核心代码

以下是项目中的一段核心代码，展示了如何实现用户登录功能：

```java
// UserController.java
@PostMapping("/login")
public ResponseEntity<?> login(@RequestBody UserLoginRequest userLoginRequest) {
    String username = userLoginRequest.getUsername();
    String password = userLoginRequest.getPassword();

    User user = userService.findByUsername(username);
    if (user == null || !passwordEncoder.matches(password, user.getPassword())) {
        return ResponseEntity.status(HttpStatus.UNAUTHORIZED).body("用户名或密码错误");
    }

    String token = jwtTokenUtil.generateToken(user);
    return ResponseEntity.ok(new JwtAuthenticationResponse(token));
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图
![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/346572/22/2934/84758/68c59c0cF09e48d16/560bcb7b7360e736.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/349844/27/3053/16287/68c59be4F01bb1455/1220627c931d0234.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/346087/8/2957/42210/68c59be4F65c2cdb6/b241e4cc23634f92.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/331427/40/12979/12817/68c59be5Ff67ff90a/1cd2a75548117aa4.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/323319/8/19590/8096/68c59be5F936c0282/a2662480fa4c79fe.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/339442/4/10479/7032/68c59be5Fa3509263/61d3dacf90d1c185.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/335050/20/12700/20197/68c59be5Fc499ccf2/49eeb99cb96d7b72.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/330503/27/12920/22697/68c59be6Fb09f4422/bd4efc0d20ac712d.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/349456/34/3076/15655/68c59be6Faa31ad5b/93293d20ead17f3b.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/322817/18/10089/27071/68c59be7F299970f3/36ed0ec5a2ad3ac2.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
