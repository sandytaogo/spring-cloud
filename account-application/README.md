# Spring Cloud User center Sample

一般来说大型互联网公司会把授权和用户信息的逻辑放到一个应用中，而这个应用我们统一称为用户中心。

用户中心不关心具体的业务逻辑，只处理用户信息相关的管理及授权登录。当第三方应用需要登录的时候，会把用户的登录请求转发到用户中心处理，处理完毕后，返回给第三方应用，第三方应用根据对应的凭证登录到系统内部。

主要功能如下:

用户登录与注册
基本信息查询与修改
从功能来看，整个用户中心还是很简单单，不过其中的逻辑还挺复杂的，比如注册功能，就要分为手机注册与邮箱注册，
手机要发送手机验证码，邮箱需要发送验证邮件，点击邮箱里面的链接跳转并进行后续注册流程，上面每步都需要业务上重新发送机制。

```
$ ./mvnw spring-boot:run
```

or

```
$ ./mvnw package
$ java -jar target/*.jar
```
