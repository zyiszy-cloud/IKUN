# IKUN - 仿B站前后端分离微服务项目

## 项目简介

这是一个基于Spring Boot + Vue.js的仿B站视频分享平台，采用微服务架构设计，实现了完整的视频分享社区功能。项目包含用户系统、视频系统、社交系统、搜索系统等多个核心模块。

## 核心功能

### 🎬 视频功能
- 视频上传（支持分片上传与断点续传）
- 视频播放、转码、压缩
- 视频点赞、收藏、分享
- 弹幕系统
- 视频推荐算法

### 👤 用户系统
- 多种登录方式（图形验证码、手机号、邮箱）
- 用户注册与身份验证
- 个人信息管理
- 用户关注与粉丝系统
- 个人主页与权限设置

### 💬 社交功能
- 视频评论与回复
- 一对一实时私聊
- 动态消息推送
- 关注UP主动态

### 🔍 搜索功能
- 视频和用户聚合搜索
- 关键字自动补全
- 搜索结果高亮显示
- 智能搜索推荐

### 🤖 AI功能
- 文生文对话
- 文生图功能
- 智能PPT生成

## 技术亮点

- **微服务架构**：基于Spring Cloud构建，服务间解耦，易于扩展和维护
- **分片上传**：支持大文件分片上传和断点续传，提升用户体验
- **实时通信**：基于WebSocket实现实时私聊和弹幕功能
- **搜索优化**：集成ElasticSearch实现高效的全文搜索
- **消息队列**：使用RocketMQ处理异步任务，提升系统性能
- **AI集成**：接入讯飞星火API，提供智能化功能
- **缓存优化**：Redis缓存热点数据，减少数据库压力
- **链路追踪**：集成Zipkin实现分布式链路追踪
  ## 项目演示
https://github.com/user-attachments/assets/109a5b6e-c354-46ef-abf2-14ffede8b725

## 技术栈

### 后端技术
- **Spring Boot** - 快速开发Java应用程序
- **Spring Security** - 安全认证与授权
- **Spring Cloud Gateway** - API网关
- **Nacos** - 服务注册与发现
- **OpenFeign** - 服务间远程调用
- **MyBatis Plus** - 数据库ORM框架
- **MySQL** - 关系型数据库
- **Redis** - 缓存数据库
- **RocketMQ** - 消息队列
- **ElasticSearch** - 搜索引擎
- **MinIO** - 对象存储
- **WebSocket** - 实时通信
- **JWT** - 身份认证
- **XXL-Job** - 分布式定时任务
- **Zipkin + Sleuth** - 链路追踪

### 前端技术
- **Vue.js** - 前端框架
- **Vue Router** - 路由管理
- **Vuex** - 状态管理
- **Element UI** - UI组件库
- **Axios** - HTTP客户端

### 开发工具
- **Swagger** - API文档
- **Druid** - 数据库连接池
- **Hutool** - Java工具类库
- **Gson** - JSON序列化
- **Jave** - 视频处理

### 第三方服务
- **讯飞星火API** - AI大模型服务

## 项目结构

```
IKUN/
├── java/                    # 后端代码
│   ├── gateway/            # 网关服务
│   ├── user_center/        # 用户中心服务
│   ├── video/              # 视频服务
│   ├── chat/               # 聊天服务
│   ├── notice/             # 消息通知服务
│   ├── search/             # 搜索服务
│   └── common/             # 公共模块
├── vue/                    # 前端代码
│   ├── src/
│   │   ├── components/     # 组件
│   │   ├── pages/          # 页面
│   │   ├── api/            # API接口
│   │   └── store/          # 状态管理
│   └── public/
└── sql.sql                 # 数据库脚本
```

## 快速开始

### 环境要求
- JDK 8+
- MySQL 8.0+
- Redis 6.0+
- Node.js 14+
- Maven 3.6+

### 后端启动
1. 导入数据库脚本 `sql.sql`
2. 修改各服务的 `application.yml` 配置文件
3. 启动各个微服务模块

### 前端启动
```bash
cd vue
npm install
npm run serve
```

## 功能展示

### 主要页面
- 🏠 首页 - 视频推荐与分类浏览
- 🎬 视频播放页 - 视频播放、弹幕、评论
- 👤 个人中心 - 用户信息、视频管理
- 💬 私信页面 - 实时聊天功能
- 🔍 搜索页面 - 智能搜索与推荐
- 🤖 AI助手 - 文生文、文生图、PPT生成

## 贡献指南

欢迎提交Issue和Pull Request来帮助改进项目！

## 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

---

⭐ 如果这个项目对你有帮助，请给个Star支持一下！
