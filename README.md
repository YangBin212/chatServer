# chatServer
基于muduo实现的可以工作在nginx tcp负载均衡环境中的集群聊天服务器和客户端源码

## 项目名称

基于muduo网络库实现的ChatServer服务器

## 平台工具

VSCode远程Linux开发，CMake构建，Linux shell输出项目编译脚本

## 项目内容

1. 使用muduo网络库作为项目的网络核心模块，提高并发网络IO服务，解耦网络和业务模块代码
2. 使用json序列化和反序列化消息作为私有通信协议
3. 配置nginx基于tcp的负载均衡，实现聊天服务器的集群功能，提高后端服务的并发能力
4. 基于redis的发布-订阅功能，实现跨服务器的消息通信
5. 使用MySQL关系型数据库作为项目数据的落地存储
6. 使用连接池提高数据库的数据存取性能
