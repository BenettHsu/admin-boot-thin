# Getting Started

> web服务脚手架(轻量版)
> 
> springboot 2.7.18


#### 1. 标配如下,自行删减

|   功能   |功能   | 描述 | version |
| ---- | ----  | ----  | ---- |
|  服务性能监控   | ✅ | actuator + prometheus | - |
|  日志   | ✅ | logback | - |
|  API文档 | ✅ | swagger | - |
|  ORM   |  ✅ |mybatis-plus + mysql | - |
|  缓存   |  ✅ |redis| - |
|  数据字典   |  ✅  |mysql| - |
|  excel导入导出   |  ✅ |alibaba/easyexcel| 2.7.x |


#### 2.项目结构
```text
.
├── pom.xml
└── src
    ├── main
    │   ├── java
    │   │   └── com
    │   │       └── admin
    │   │           └── adminboothin
    │   │               ├── AdminBooThinApplication.java
    │   │               ├── common  //公共区
    │   │               │   ├── cache  //公共缓存
    │   │               │   ├── component  //公共组件
    │   │               │   │   ├── dict  //数据字典
    │   │               │   │   └── excel //excel导入导出
    │   │               │   ├── constant  //常量
    │   │               │   └── utils  //自定义工具类
    │   │               ├── conf  //配置区
    │   │               │   ├── aspect  //aop切面
    │   │               │   ├── async  //异步线程(任务)池
    │   │               │   ├── exception //异常
    │   │               │   ├── filter  //过滤器
    │   │               │   ├── interceptor  //拦截器
    │   │               │   ├── jackson  //正反序列化
    │   │               │   ├── mp //mybatis-plus
    │   │               │   ├── properties  //配置文件值映射
    │   │               │   ├── redis
    │   │               │   ├── rest  //restTemplate
    │   │               │   └── swagger  //API文档
    │   │               ├── controller
    │   │               ├── mapper
    │   │               ├── pojo
    │   │               │   ├── annotation  //自定义注解
    │   │               │   ├── bo  //业务对象
    │   │               │   ├── dto  //传输对象
    │   │               │   ├── entity  //db实体对象
    │   │               │   ├── enums  //枚举
    │   │               │   ├── qo  //查询对象
    │   │               │   └── vo  //试图对象
    │   │               ├── schedule  //定时任务
    │   │               └── service
    │   │                   └── impl
    │   └── resources
    │       ├── application-dev.yml
    │       ├── application-prod.yml
    │       ├── application-test.yml
    │       ├── application.yml
    │       ├── logback.xml  //logback配置
    │       └── mapper  //mybatis-plus xml文件
    └── test
        └── java
            └── com
                └── admin
                    └── adminboothin
                        └── AdminBooThinApplicationTests.java

```


