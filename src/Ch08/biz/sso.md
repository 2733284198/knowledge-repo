# 单点登陆

## SSO

Single sign-on (SSO) is an authentication scheme that allows a user to log in with a single ID and password to any of several related, yet independent, software systems.

##

IDP

Service Provider

Identity provider offers user authentication as a service. In simple words, you can add and manage your user accounts, groups in an Identity Provider which gives you a way to authenticate your users while accessing any of your services.

一般提出单点服务的同时意味着要解决下面的三个问题

- 单点登录
- 权限中心
- 信息聚合

有以下几种类型的设计方案，按照设计复杂度由低到高

1. 仅登陆方案
2. 用户网关方案
3. CAS 方案

一般惯用做法如下

1. 注册一般走子服务
3. 登陆走单点登陆
2. 注销一般做全局
4. 权限一般在子服务这一层，做的精细一些的话可以新增 IAM 类型做权限校验
5. 检索某个服务 通过接口入参来控制 网关设计上 有个聚合查询的参数 可以参考这个


