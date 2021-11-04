<p align="center"><img src="./documents/readme/logo.png" height="150" width="150" alt="logo"/></p>
<h2 align="center">简洁优雅 · 稳定高效 | 宁静致远 · 精益求精 </h2>
<h3 align="center">Eurynome Cloud 微服务架构</h3>

---

<p align="center">
    <a href="https://www.oracle.com/java/technologies/javase-downloads.html" target="_blank"><img src="https://img.shields.io/badge/JDK-1.8%2B-green" alt="JDK 1.8+"></a>
    <a href="https://spring.io/projects/spring-boot" target="_blank"><img src="https://img.shields.io/badge/Spring%20Boot-2.5.6-blue" alt="Spring Boot 2.5.6"></a>
    <a href="https://spring.io/projects/spring-cloud" target="_blank"><img src="https://img.shields.io/badge/Spring%20Cloud-2020.0.4-blue" alt="Spring Cloud 2020.0.4"></a>
    <a href="https://github.com/alibaba/spring-cloud-alibaba" target="_blank"><img src="https://img.shields.io/badge/Spring%20Cloud%20Alibaba-2021.1-blue" alt="Spring Cloud Alibaba 2021.1"></a>
    <a href="https://nacos.io/zh-cn/index.html" target="_blank"><img src="https://img.shields.io/badge/Nacos-2.0.3-brightgreen" alt="Nacos 2.0.3"></a>
    <a href="./LICENSE"><img src="https://img.shields.io/badge/License-Apache--2.0-blue" alt="License Apache 2.0"></a>
    <a href="https://blog.csdn.net/Pointer_v" target="_blank"><img src="https://img.shields.io/badge/Author-%E7%A0%81%E5%8C%A0%E5%90%9B-orange" alt="码匠君"></a>
    <a href="#" target="_blank"><img src="https://img.shields.io/badge/Version-2.5.6.20-red" alt="Version 2.5.6.20"></a>
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

Eurynome Cloud是一款企业级微服务架构和服务能力开发平台。基于Spring Boot 2.5.6、Spring Cloud 2020.0.4、Spring Cloud Alibaba 2021.1、Nacos 2.0.3 等最新版本开发，遵循SpringBoot编程思想，高度模块化和可配置化。具备服务发现、配置、熔断、限流、降级、监控、多级缓存、分布式事务、工作流等功能，代码简洁，架构清晰，非常适合学习和企业作为基础框架使用。

## 平台定位

- 构建成熟的、完善的、全面的，基于 OAuth2 的、前后端分离的微服务架构解决方案。
- 面向企业级应用和互联网应用设计开发，既兼顾传统项目的微服务化，又满足互联网应用开发建设、快速迭代的使用需求。
- 平台架构使用微服务领域及周边相关的各类新兴技术或主流技术进行建设，是帮助快速跨越架构技术选型、研究探索阶段的利器。
- 代码简洁规范、结构合理清晰，是新技术开发应用的典型的、综合性案例，助力开发人员对新兴技术的学习和掌握。

## Gitee Star趋势图

[![Giteye chart](https://chart.giteye.net/gitee/herodotus/eurynome-cloud/254B32UX.png)](https://giteye.net/chart/254B32UX)

## [1]、总体架构

![输入图片说明](./documents/readme/architecture.jpg)

> 部分功能演示，正在逐步添加

### （1） 方法级动态权限

![输入图片说明](./documents/readme/preview/oauth2expression.gif)

### （2） 服务调用链监控

![输入图片说明](./documents/readme/preview/skywalking.gif)

## [2]、功能介绍

<a href="https://www.herodotus.cn">详情见在线文档</a>

## [3]、技术栈和版本说明

### （1）Spring全家桶及核心技术版本

| 组件                 | 版本     |
| -------------------- | -------- |
| Spring Boot          | 2.5.6    |
| Spring Cloud         | 2020.0.4 |
| Spring Cloud Alibaba | 2021.1   |
| Spring Boot Admin    | 2.5.3    |
| Nacos                | 2.0.3    |
| Sentinel             | 1.8.0    |
| Seata                | 1.3.0    |

> Spring 全家桶版本对应关系，详见：[版本说明](https://github.com/alibaba/spring-cloud-alibaba/wiki/%E7%89%88%E6%9C%AC%E8%AF%B4%E6%98%8E)

### （2）所涉及的相关的技术：

- 持久层框架： Spring Data Jpa & Mybatis Plus
- API网关：Spring Cloud Gateway
- 服务注册&发现和配置中心: Alibaba Nacos
- 服务消费：Spring Cloud OpenFeign & RestTemplate & OkHttps
- 负载均衡：Spring Cloud Loadbalancer
- 服务熔断&降级&限流：Alibaba Sentinel
- 服务监控：Spring Boot Admin
- 消息队列：使用Spring Cloud消息总线Spring Cloud Bus 默认Kafka 适配RabbitMQ
- 链路跟踪：Skywalking
- 分布式事务：Seata
- 数据缓存：JetCache + Redis + Caffeine, 自定义多级缓存
- 数据库： Postgresql，MySQL，Oracle ...
- JSON序列化：Jackson & FastJson
- 文件服务：阿里云OSS/Minio
- 数据调试：p6spy
- 日志中心：ELK
- 日志收集：Logstash Logback Encoder

## [4]、 版本号说明

本系统版本号，分为四段。

- 第一段和第二段，与Spring Boot 版本对应，根据采用的Spring Boot版本变更。例如，当前采用Spring Boot 2.4.6版本，那么就以2.4.X.X开头
- 第三段，表示系统功能的变化
- 第四段，表示系统功能维护及优化情况

## [5]、工程结构

``` 
eurynome-cloud
├── configurations -- 配置文件脚本和统一Docker build上下文目录
├── dependencies -- 工程Maven顶级依赖，统一控制版本和依赖
├── packages -- 基础通用依赖包
├    ├── eurynome-cloud-assistant -- Spring相关公共辅助工具、注解相关工具代码组件
├    ├── eurynome-cloud-data -- 数据持久化、数据缓存以及Redis等数据处理相关代码组件
├    ├── eurynome-cloud-kernel -- 微服务接入平台必备组件
├    ├── eurynome-cloud-oauth -- OAuth2通用代码
├    ├── eurynome-cloud-oauth-starter -- 自定义OAuth2 Starter，Athena单体版核心Starter
├    ├── eurynome-cloud-rest -- Rest相关代码组件
├    ├── eurynome-cloud-sercurity -- Security通用代码
├    ├── eurynome-cloud-starter -- 微服务核心Starter
├    └── eurynome-cloud-websocket -- WebSocket核心代码包
├── platform -- 平台核心服务
├    ├── eurynome-cloud-gateway -- 服务网关
├    ├── eurynome-cloud-management -- Spring Boot Admin 监控服务
├    └── eurynome-cloud-uaa -- 统一认证模块
├── services -- 平台业务服务
├    ├── eurynome-cloud-upms-api -- 通用用户权限api 
├    ├── eurynome-cloud-upms-logic -- 通用用户权限service
├    ├── eurynome-cloud-upms-rest -- 通用用户权限rest 接口
├    ├── eurynome-cloud-upms-ability -- 通用用户权限服务
├    ├── eurynome-cloud-upms-rest -- 工作流基础代码包
└──  └── eurynome-cloud-bpmn-ability -- 工作流服务 
```

## [6]、项目地址

- 后端Gitee地址：[https://gitee.com/herodotus/eurynome-cloud](https://gitee.com/herodotus/eurynome-cloud)
- 后端Github地址：[https://github.com/herodotus-cloud/eurynome-cloud](https://github.com/herodotus-cloud/eurynome-cloud)
- 单体版示例工程：[https://gitee.com/herodotus/eurynome-cloud-athena](https://gitee.com/herodotus/eurynome-cloud-athena)
- 前端Gitee地址：[https://gitee.com/herodotus/eurynome-cloud-ui](https://gitee.com/herodotus/eurynome-cloud-ui)

## [7]、用户权益

- 允许免费用于学习、毕设、公司项目、私活等。
- 遵循Apache-2.0开源协议

## [8]、交流反馈

- 欢迎提交[ISSUS](https://gitee.com/herodotus/eurynome-cloud/issues) ，请写清楚问题的具体原因，重现步骤和环境(上下文)
- 博客：https://blog.csdn.net/Pointer_v
- 邮箱：herodotus@aliyun.com
- QQ群：922565573

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
