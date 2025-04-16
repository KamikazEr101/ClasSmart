# 🤖 ClasSmart—灵分

## 📚 简介 | Introduction

`ClasSmart—灵分`是一款智能垃圾分类系统。  

用户仅需要提交待分类的图片，即可得到分类结果。 

## 🌐 一套代码，多端适配 | Multiple Endpoints

<img src="./assets/appshow_ap.png" style="zoom:40%;" />


## 🚀 使用方法 | Usage Method

1. **浏览器输入前端地址**

2. **传入待分类图片**

## 📋 功能列表 | Function List

| 功能                                                         |
| :----------------------------------------------------------- |
| **智能鉴别具体垃圾类型**                                     |
| 采用 `Autogen` 智能体**智能识别恶意图片**，防止污染数据库与模型 |
| **定时**将用户传入图片与反馈打包为数据集，进行 `Pytorch` 模型**复训练** |
| 使用 `Redis` **分布式锁**，支持**多实例单数据源**分布式部署    |
| 采用 `Redis` 的**分布式限流策略**，总体使用**令牌桶算法**限流，并对**独立IP**实施**黑名单**策略 |
| 前端使用 `React` 框架，优化**首屏加载**与**SEO**               |

## 🛠️ 涉及技术栈 | Tech Stack

| 模块       | 技术/组件 |
| ---------- | --------- |
| [前端](https://github.com/KamikazEr101/ClasSmart_frontend) | `React` |
| [java 后端](https://github.com/KamikazEr101/ClasSmart_backend_java) | `SpringBoot`、`SpringMVC`、`Mybatis`、`Redis`、 `Minio` |
| [python 后端](https://github.com/Ying-Luan/ClasSmart_backend_python) | `Pytorch`、`Autogen`、`FastAPI` |



## 🔮 未来展望 | Future Outlook

`ClasSmart—灵分` 计划在未来进一步**优化分类算法**，引入**更先进的深度学习模型**以提高准确率，实现企业级分布式部署。同时，计划扩展至更多智能设备，打造物联网垃圾分类生态系统，并推出多语言支持以服务全球用户。



| 模块        | 未来方向                                                     |
| ----------- | ------------------------------------------------------------ |
| [前端](https://github.com/KamikazEr101/ClasSmart_frontend)        | 通过持续迭代 `React` 框架以增强其性能、组件复用性和虚拟 DOM 的效率，结合先进的状态管理策略，旨在构建一个更加高效、可维护且用户体验优化的前端应用 |
| [java 后端](https://github.com/KamikazEr101/ClasSmart_backend_java)   | 通过构建 `Redis` 集群以提供高性能的缓存服务，结合`Spring Cloud` 框架实现微服务架构与分布式事务管理，进而优化数据库表结构并采用 `MinIO` 的分布式部署策略，旨在构建一个高效、可扩展且具备高可用性的现代化软件系统 |
| [python 后端](https://github.com/Ying-Luan/ClasSmart_backend_python) | 通过采用先进的分布式计算架构，将模型的推理和再训练过程解耦，并分别部署于专用的计算节点上。优化硬件资源的分配与使用效率，提升系统吞吐量与响应速度。引入高效的 `LLM 智能体框架`，通过本地部署经过微调的 LLM，实现服务效率与安全性的双重提升。 |