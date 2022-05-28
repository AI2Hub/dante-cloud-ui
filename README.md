<p align="center"><img src="./documents/readme/logo.png" height="150" width="150" alt="logo"/></p>
<h2 align="center">简洁优雅 · 稳定高效 | 宁静致远 · 精益求精 </h2>
<h3 align="center">Eurynome Cloud 微服务架构</h3>

---

<p align="center">
    <a href="https://www.oracle.com/java/technologies/javase-downloads.html" target="_blank"><img src="https://shields.io/badge/JDK-17%2B-green" alt="JDK 17+"></a>
    <a href="https://spring.io/projects/spring-boot" target="_blank"><img src="https://shields.io/badge/Spring%20Boot-2.7.0-blue" alt="Spring Boot 2.7.0"></a>
    <a href="https://spring.io/projects/spring-cloud" target="_blank"><img src="https://shields.io/badge/Spring%20Cloud-2021.0.2-blue" alt="Spring Cloud 2021.0.2"></a>
    <a href="https://github.com/alibaba/spring-cloud-alibaba" target="_blank"><img src="https://shields.io/badge/Spring%20Cloud%20Alibaba-2021.0.1.0-blue" alt="Spring Cloud Alibaba 2021.0.1.0"></a>
    <a href="https://github.com/spring-projects/spring-authorization-server" target="_blank"><img src="https://img.shields.io/badge/Spring%20Authorization%20Server-0.3.0-blue" alt="Spring Authorization Server 0.3.0"></a>
    <a href="https://nacos.io/zh-cn/index.html" target="_blank"><img src="https://shields.io/badge/Nacos-2.1.0-brightgreen" alt="Nacos 2.1.0"></a>
    <a href="./LICENSE"><img src="https://shields.io/badge/License-Apache--2.0-blue" alt="License Apache 2.0"></a>
    <a href="https://blog.csdn.net/Pointer_v" target="_blank"><img src="https://shields.io/badge/Author-%E7%A0%81%E5%8C%A0%E5%90%9B-orange" alt="码匠君"></a>
    <a href="#" target="_blank"><img src="https://shields.io/badge/Version-2.7.0.10-red" alt="Version 2.7.0.10"></a>
    <a href="https://gitee.com/herodotus/eurynome-cloud"><img src="https://gitee.com/herodotus/eurynome-cloud/badge/star.svg?theme=dark" alt="Gitee star"></a>
    <a href="https://gitee.com/herodotus/eurynome-cloud"><img src="https://gitee.com/herodotus/eurynome-cloud/badge/fork.svg?theme=dark" alt="Gitee fork"></a>
</p>

<p align="center">
    <a href="https://github.com/herodotus-cloud/eurynome-cloud">Github 仓库</a> &nbsp; | &nbsp;
    <a href="https://gitee.com/herodotus/eurynome-cloud">Gitee 仓库</a> &nbsp; | &nbsp;
    <a href="https://www.herodotus.cn">文档</a>
</p>

<h1 align="center"> 如果您觉得有帮助，请点右上角 "Star" 支持一下，谢谢！</h1>

---

## 企业级技术中台微服务架构与服务能力开发平台

Eurynome Cloud 是一款企业级微服务架构和服务能力开发平台。基于 Spring Boot 2.7.0、Spring Cloud 2021.0.3、Spring Cloud Alibaba 2021.0.1.0、Nacos 2.1.0 等最新版本开发，遵循 SpringBoot 编程思想，高度模块化和可配置化。具备服务发现、配置、熔断、限流、降级、监控、多级缓存、分布式事务、工作流等功能，代码简洁，架构清晰，非常适合学习和企业作为基础框架使用。

## 平台定位

-   构建成熟的、完善的、全面的，基于 OAuth2 的、前后端分离的微服务架构解决方案。
-   面向企业级应用和互联网应用设计开发，既兼顾传统项目的微服务化，又满足互联网应用开发建设、快速迭代的使用需求。
-   平台架构使用微服务领域及周边相关的各类新兴技术或主流技术进行建设，是帮助快速跨越架构技术选型、研究探索阶段的利器。
-   代码简洁规范、结构合理清晰，是新技术开发应用的典型的、综合性案例，助力开发人员对新兴技术的学习和掌握。

## 重要说明

Eurynome Cloud 自 v2.7.0.20 版本，开始全面使用 JDK 17。自该版本以后，系统代码将不再兼容 JDK 8，敬请悉知！

升级使用 JDK 17 的主要原因：

1. Spring Authorization Server 0.3.0 版本，已经开始使用 JDK 11 进行代码编译。该版本在 JDK 8 下已无法编译成功，想要使用必须要升级 JDK 版本。
2. 2022 年 11 月，Spring Boot 3 将会发布，最低版本要求 JDK 17。因此，直接将 JDK 版本升级至 17，同时为升级至 Spring Boot 3 提前做铺垫准备。

## 升级说明

在 `Spring Security OAuth2` 彻底停止维护、Spring Boot 2.7.0 正式发布之时，又恰逢 `Eurynome Cloud` 开源一周年之际，推出基于 Spring Authorization Server 0.3.0、Spring Boot 2.7.0、Spring Cloud 2021.0.2、Spring Cloud Alibaba 2021.0.1.0 和 Nacos 2.1.0 的全新正式版本。

## 新版特点

-   基于 `Spring Authorization Server` 深度定制:

    -   基于 `Spring Data JPA`，重新构建 `Spring Authorization Server` 基础数据存储代码，替代原有 JDBC 数据访问方式，破除 `Spring Authorization Server` 原有数据存储局限，扩展为更符合实际应用的方式和设计。

    -   基于 `Spring Authorization Server`，在 OAuth 2.1 规范基础之上，增加自定义“密码”认证模式，以兼容现有基于 OAuth 2 规范的、前后端分离的应用。
    -   基于 `Spring Authorization Server`，在 OAuth 2.1 规范基础之上，增加自定义 Social Credentials 认证模式，支持手机短信验证码、微信小程序、第三方应用登录。
    -   遵照 `Spring Security 5` 以及 `Spring Authorization Server` 的代码规范，进行 OAuth2 认证服务器核心代码的开发，遵照其使用 Jackson 反序列化的方式， 增加大量自定义 Jackson Module。
    -   支持 `Spring Authorization Server` 的标准的 Token 加密校验方式外，还了增加支持自定义证书的 Token 加密方式，可通过配置动态修改
    -   支持 OAuth2 OIDC 认证模式，补充前端 OIDC 认证相关配置操作，以及对应的 /userinfo 接口调用支持 和 客户端注册支持
    -   支持 OAuth2 Authorization Code PKCE 认证模式
    -   扩展 `Spring Authorization Server` 默认的 `Client Credentials` 模式，实现 Refresh Token 的创建。
    -   扩展 `Spring Authorization Server` 默认的 `Client Credentials` 模式，实现真正的使用 Scope 权限对接口进行验证。 增加客户端 Scope 的权限配置功能，并与已有的用户权限体系解耦
    -   自定义 `Spring Authorization Server` 授权码模式登录认证页面和授权确认页面，授权码模式登录采用数据加密传输。支持多种验证码类型，暂不支持行为验证码。

-   代码结构的大规模调整和优化：
    -   对原有代码进行了深度的“庖丁解牛”，严格遵照“单一职责”原则，根据各个组件的职责以及用途，将整个工程拆解细化为多个各自独立组件模块，在最大程度上降低代码间的耦合，也更容易聚焦和定位问题。
    -   将通用化组件提取为独立工程，独立编译、按需选用，极大的降低系统主工程代码量。相关组件也已上传至 Maven 中央仓库，降低系统主工程工程代码编译耗时，改进和提升 CICD 效率，
    -   原有主工程代码结构也进行了深化调整，代码分包更加合理，代码逻辑也更加清晰。

## 细节品鉴

俗话说：不看“广告”，看“疗效”。本项目除了将微服务应用涉及的“标准动作”实现之外，也尽可能的“推陈出新”，增加大量细节内容，不仅更加“包容兼顾”，也更利于开发使用。加之本着不重复“造轮子”的原则，在能使用成熟组件代码的情况下，绝不重复实现相关代码，代码实现简洁、可读性高。本项目后端代码最为闪耀，细节满满，值得品鉴。

-   遵照 Spring Boot 标准化的方式，装配模块和相关代码。大量使用自定义 @ConditionOnXXX、@EnableXXX 注解，实现配置的动态、灵活的注入。
-   大量使用 Spring 和 Spring Boot 自身的事件驱动、InitializingBean 等机制，实现相关代码逻辑，代码更加清晰、逻辑更加简洁、维护更加方便。
-   大量使用基于 Spring Boot 的策略模式和工厂模式，让同质的功能可以条件化、策略化的注入，便于根据使用者自身需求动态变更支持代码。
-   自定义多级缓存，与 `Spring Data JPA` 有机整合，有效解决 `Spring Cache` 等缓存对条件查询、分页查询支持不够便捷的问题。
-   基于数字信封原理，综合使用对称和非对称加密算法，实现前后端数据加密传输。支持国密算法 SM2 和 SM4 混合以及标准的 RSA 和 AES 混合。可通过配置文件配置进行切换，通过注解灵活个性化设置。
-   基于自定义 Session 实现秘钥动态生成、加密传输、一人一钥的安全机制，可通过配置动态开启和关闭。不是使用传统 Filter 方式进行加密处理，而是扩展 @RequestParam 等注解实现逻辑实现数据加解密。支持使用自定义注解灵活配置加密策略以及数据缓存策略。
-   遵照知名开源项目方式，设计 Maven Dependencies 依赖继承结构，结构清晰明了、依赖干净无冗余、修改维护便捷。各个模块以最小化模式进行包的依赖，简洁清爽，逻辑清晰，不会出现依赖循环问题。
-   个性化设计 Nacos 配置文件关系及逻辑，将高频修改配置参数统一提取，仅需在同一配置文件修改少量参数即可完成环境搭建和配置控制，降低修改参数的出错率。
-   将 Maven、Spring Boot、Nacos、Docker 等内容涉及的多环境配置有机融合和关联，可以方便地在各个环境中切换。
-   包含 Git 提交信息打包、源代码生成、容器打包等多种 Maven 构建插件及配置，相关信息也可在 `Spring Boot Admin` 展现。
-   集成较多同质组件或代码实现的可选择化使用，选择更丰富，使用更灵活

> 更多细节，欢迎对本项目进行深入了解

## 额外说明

1. 本项目以后将主要维护 `Spring Authorization Server` 版本，原有基于 `Spring Security OAuth2` 的版本已经移至 spring-security-oauth2 分支，可以从该分支或发行版页面获取历史版本继续使用。后期会根据 ISSUE 以及使用用户反馈情况，再行决定是否继续维护 `Spring Security OAuth2` 版本。
2. 最新版本代码，暂时继续沿用原有基于 Vue2、Vuetify2、Typescript 开发的前端系统。基于 Vue3、Vite2、Vuetify3、Pinia 等新版前端正在加进开发中，由于 Vuetify3 版本发布跳票以及部分已有组件的缺失，导致新版前端开发延后。
3. 原有基于 Vue2、Vuetify2、Typescript 开发的前端，由于使用了过渡性 Typescript IOC 组件，以及依赖组件版本限制等问题，初次接触该项目在编译过程中会出现一些问题，请移步至本项目在线文档，详见“常见问题”章节。

### 为什么前端框架选择 Vuetify

在本项目建设初期，选择 Vuetify 作为前端组件，主要原因就是其是 Material 样式的 UI 组件以及更新频率较高、维护的持续性较好。经过几年的使用，发现该套组件库封装度很高，组件的属性配置丰富、使用灵活、可定制性强、学习使用曲线低。

特别是 Vuetify 对常见的样式使用和布局处理进行了深度封装，不需在样式和布局设计上投入大量精力，通过简单的属性配置就可以做出比较好看的界面。这一点对不擅长前端和美工设计、想快速实现前端的后端人员非常友好。

在进行 Vue3 版本开发之前，也对 Element Plus、Naive UI 等组件库进行了对比，也基于评分较高的开源后台模版进行了尝试性开发。发现大多数组件库相比 Vuetify，组件配置属性都少了很多，没有 Vuetify 灵活，而且都需要自己编写大量的样式，甚至需要自己实现常规组件。因此，新版本前端最终仍旧选择使用 Vuetify。

## 重要信息

> 不一定非要捐赠或者参与编写代码，才是参与开源项目的正确方式。点个 `Star`、提个格式规范的 ISSUE，也是在积极参与开源项目，更是对作者莫大的支持和鼓励。

> 开发新手在群内提问或新开 Issue 提问前，请先阅读 [【提问的智慧】](https://www.herodotus.cn/others/question/)，并确保认真、详细地查阅过本项目 [【在线文档】](https://www.herodotus.cn)，避免浪费大家的宝贵时间；

## [1]、总体架构

![输入图片说明](./documents/readme/architecture.jpg)

> 部分功能演示，正在逐步添加

### （1） 方法级动态权限

![输入图片说明](./documents/readme/preview/oauth2expression.gif)

### （2） 服务调用链监控

![输入图片说明](./documents/readme/preview/skywalking.gif)

### （3） 灵活定制验证码

-   滑块拼图验证码

![滑块拼图验证码](./documents/readme/captcha-jigsaw.png)

-   文字点选验证码

![文字点选验证码](./documents/readme/captcha-word-click.png)

## [2]、功能介绍

<a href="https://www.herodotus.cn">详情见在线文档</a>

## [3]、技术栈和版本说明

### （1）Spring 全家桶及核心技术版本

| 组件                        | 版本       |
| --------------------------- | ---------- |
| Spring Boot                 | 2.7.0      |
| Spring Cloud                | 2021.0.3   |
| Spring Cloud Alibaba        | 2021.0.1.0 |
| Spring Authorization Server | 0.3.0      |
| Spring Boot Admin           | 2.6.7      |
| Nacos                       | 2.1.0      |
| Sentinel                    | 1.8.3      |
| Seata                       | 1.3.0      |

> Spring 全家桶版本对应关系，详见：[版本说明](https://github.com/alibaba/spring-cloud-alibaba/wiki/%E7%89%88%E6%9C%AC%E8%AF%B4%E6%98%8E)

### （2）所涉及的相关的技术：

-   持久层框架： Spring Data Jpa & Mybatis Plus
-   API 网关：Spring Cloud Gateway
-   服务注册&发现和配置中心: Alibaba Nacos
-   服务消费：Spring Cloud OpenFeign & RestTemplate & OkHttps
-   负载均衡：Spring Cloud Loadbalancer
-   服务熔断&降级&限流：Alibaba Sentinel
-   服务监控：Spring Boot Admin
-   消息队列：使用 Spring Cloud 消息总线 Spring Cloud Bus 默认 Kafka 适配 RabbitMQ
-   链路跟踪：Skywalking
-   分布式事务：Seata
-   数据缓存：JetCache + Redis + Caffeine, 自定义多级缓存
-   数据库： Postgresql，MySQL，Oracle ...
-   JSON 序列化：Jackson & FastJson
-   文件服务：阿里云 OSS/Minio
-   数据调试：p6spy
-   日志中心：ELK
-   日志收集：Logstash Logback Encoder

## [4]、 版本号说明

本系统版本号，分为四段。

-   第一段和第二段，与 Spring Boot 版本对应，根据采用的 Spring Boot 版本变更。例如，当前采用 Spring Boot 2.4.6 版本，那么就以 2.4.X.X 开头
-   第三段，表示系统功能的变化
-   第四段，表示系统功能维护及优化情况

## [5]、工程结构

```
eurynome-cloud
├── configurations -- 配置文件脚本和统一Docker build上下文目录
├── dependencies -- 工程Maven顶级依赖，统一控制版本和依赖
├── packages -- 基础通用依赖包
├    ├── eurynome-cloud-assistant -- Spring相关公共辅助工具、注解相关工具代码组件
├    ├── eurynome-cloud-cache -- Cache和Redis工具模块组件
├    ├── eurynome-cloud-captcha -- 验证码模块组件
├    ├── eurynome-cloud-data -- 数据持久化等数据处理相关代码组件
├    ├── eurynome-cloud-kernel -- 微服务接入平台必备组件
├    ├── eurynome-cloud-message -- 消息处理相关代码组件
├    ├── eurynome-cloud-oauth -- OAuth2通用代码
├    ├── eurynome-cloud-oauth-starter -- 自定义OAuth2 Starter，Athena单体版核心Starter
├    ├── eurynome-cloud-pay -- 支付核心组件包
├    ├── eurynome-cloud-rest -- Rest相关代码组件
├    ├── eurynome-cloud-sercurity -- Security通用代码
├    ├── eurynome-cloud-starter -- 微服务核心Starter
├    ├── eurynome-cloud-web -- Web 应用基础组件
├    └── eurynome-cloud-websocket -- WebSocket核心代码包
├── platform -- 平台核心服务
├    ├── eurynome-cloud-gateway -- 服务网关
├    ├── eurynome-cloud-monitor -- Spring Boot Admin 监控服务
├    └── eurynome-cloud-uaa -- 统一认证模块
├── services -- 平台业务服务
├    ├── eurynome-cloud-upms-logic -- 通用用户权限service
├    ├── eurynome-cloud-upms-rest -- 通用用户权限rest 接口
├    ├── eurynome-cloud-upms-ability -- 通用用户权限服务
├    ├── eurynome-cloud-upms-rest -- 工作流基础代码包
└──  └── eurynome-cloud-bpmn-ability -- 工作流服务
```

## [6]、项目地址

-   后端 Gitee 地址：[https://gitee.com/herodotus/eurynome-cloud](https://gitee.com/herodotus/eurynome-cloud)
-   后端 Github 地址：[https://github.com/herodotus-cloud/eurynome-cloud](https://github.com/herodotus-cloud/eurynome-cloud)
-   单体版示例工程：[https://gitee.com/herodotus/eurynome-cloud-athena](https://gitee.com/herodotus/eurynome-cloud-athena)
-   前端 Gitee 地址：[https://gitee.com/herodotus/eurynome-cloud-ui](https://gitee.com/herodotus/eurynome-cloud-ui)

## [7]、用户权益

-   允许免费用于学习、毕设、公司项目、私活等。
-   遵循 Apache-2.0 开源协议

## [8]、交流反馈

-   欢迎提交[ISSUS](https://gitee.com/herodotus/eurynome-cloud/issues) ，请写清楚问题的具体原因，重现步骤和环境(上下文)
-   博客：https://blog.csdn.net/Pointer_v
-   邮箱：herodotus@aliyun.com
-   QQ 群：922565573

## [9]、界面预览

<table>
    <tr>
        <td><img src="./documents/readme/ui1.png" alt="前端界面1"/></td>
        <td><img src="./documents/readme/ui2.png" alt="前端界面2"/></td>
    </tr>
    <tr>
        <td><img src="./documents/readme/ui3.png" alt="前端界面3"/></td>
        <td><img src="./documents/readme/camunda.png" alt="Camunda 工作流在线编辑器"/></td>
    </tr>
    <tr>
        <td><img src="./documents/readme/nacos.png" alt="Nacos示例界面"/></td>
        <td><img src="./documents/readme/elk.png" alt="日志中心示例界面"/></td>
    </tr>
    <tr>
        <td><img src="./documents/readme/oauth2-login1.png" alt="OAuth2 效果示例"/></td>
        <td><img src="./documents/readme/sentinel.png" alt="Sentinel 效果示例"/></td>
    </tr>
    <tr>
        <td><img src="./documents/readme/spring-boot-admin-1.png" alt="Spring Boot Admin 效果示例1"/></td>
        <td><img src="./documents/readme/spring-boot-admin-2.png" alt="Spring Boot Admin 效果示例2"/></td>
    </tr>
    <tr>
        <td><img src="./documents/readme/skywalking.png" alt="Skywalking 效果示例1"/></td>
        <td><img src="./documents/readme/skywalking2.png" alt="Skywalking 效果示例2"/></td>
    </tr>
</table>

## [10]、鸣谢

-   [Soybean Admin](https://gitee.com/honghuangdc/soybean-admin)
-   [Vue Next Admin](https://gitee.com/lyt-top/vue-next-admin)
-   [Vue VBen Admin](https://gitee.com/annsion/vue-vben-admin)
