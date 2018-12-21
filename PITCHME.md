> 让系统活起来

# Apollo

---
> 背景

* 随着程序功能的日益复杂，程序的配置日益增多：各种功能的开关、参数的配置、服务器的地址……

* 对程序配置的期望值也越来越高：配置修改后实时生效，灰度发布，分环境、分集群管理配置，完善的权限、审核机制……

* 在这样的大环境下，传统的通过配置文件、数据库等方式已经越来越无法满足开发人员对配置管理的需求。

* Apollo配置中心应运而生！

---


> What is Apollo

* 携程框架部门开源的统一应用配置中心
* 支持4个维度管理配置（Key-Value）
     * application (应用)
    * environment (环境)
    * cluster (集群)
    * namespace (命名空间)

---

> What is Configuration

- 配置是独立于程序的只读变量
  - DB Connection Str、Thread Pool Size、Buffer Size、Request
Timeout、Feature Switch、Server Urls等
- 配置伴随应用的整个生命周期
    - 启动时读取配置，运行时根据配置调整行为
- 配置可以有多种加载方式
    - 程序内部hard code，配置文件，环境变量，启动参数，基于数据库等
- 配置需要治理
    - 权限控制、发布审核
    - 不同环境、集群配置管理

---

> 总体设计

![总体设计](https://github.com/KevinCai76/points/blob/master/Images/overall-architecture.png?raw=true)

+++

>  客户端设计

![客户端设计](https://github.com/KevinCai76/points/blob/master/Images/client-architecture.png?raw=true)

---

# GitPitch
* what is GitPitch
* [show me](https://gitpitch.com/KevinCai76/points)
---
 
---

## 更多演示

 - [Show Me](https://gitpitch.com/gitpitch/the-template#/)
 - [See Code](https://github.com/gitpitch/the-template)
