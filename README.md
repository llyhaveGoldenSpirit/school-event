# 校园事件管理系统
## 技术栈：
Spring、SpringMVC、Mybatis、SpringBoot、MySQL、Redis、Vue3、Element
## 描述：
该项目是一个应用于学校场景的信息发布与管理平台，在登录注册后可以发布和管理信息，也可以管理个人信息，实现了基本的校园事件和用户信息的增删改查。
![image](https://github.com/llyhaveGoldenSpirit/school-event/assets/137288074/e238567f-6d17-48ee-8aee-b478e20d0fcb)
![image](https://github.com/llyhaveGoldenSpirit/school-event/assets/137288074/5c3e2259-8122-4449-bd68-31e52bf02231)

除此之外：
- 采用JWT令牌技术和自定义拦截器，实现了用户认证功能，并通过ThreadLocal优化鉴权逻辑；
- 利用redis解决了修改密码后旧令牌依旧有效的安全隐患，实现了令牌的及时更新和校验；
- 应用Spring Validation完成了接口参数的合法校验，自定义注解state实现了对文章状态的校验；
- 使用pinia来保存token，让多个页面共享状态，解决刷新页面token丢失的问题。
