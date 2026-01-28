

# KM2

## 项目简介

KM2 是一个基于 Web 技术栈开发的 Android 移动端考试练习应用。项目采用混合开发模式（Hybrid App），通过 Cordova 将基于 Bootstrap 的响应式 Web 页面打包为原生移动应用。

该应用主要面向考试学习场景，提供了模拟考试、计时计分、项目分类展示以及用户设置等功能。

## 核心功能

- **模拟考试系统**：包含实时计时器、进度条、分数统计、扣分操作及结束考试流程。
- **项目卡片管理**：以卡片形式展示不同类别的考试项目（红/黄/蓝/绿四色分类），界面清晰直观。
- **个人设置**：提供应用基础设置选项（如音效、振动等开关）。
- **互动社区**：集成联系页面，支持二维码展示及视频弹窗功能。
- **UI/UX 设计**：采用现代玻璃拟态（Glassmorphism）导航栏设计，配合 Bootstrap 5 图标库。

## 技术架构

- **前端技术**：HTML5, CSS3 (Bootstrap 5 + 自定义样式), JavaScript
- **UI 框架**：[Bootstrap 5](https://getbootstrap.com/) (CSS & JS)
- **图标库**：[Bootstrap Icons](https://icons.getbootstrap.com/)
- **打包框架**：[Apache Cordova](https://cordova.apache.org/)
- **目标平台**：Android

## 项目结构

```
.
├── config.xml                 # Cordova 配置文件
├── my-release-key.keystore    # Android 应用签名密钥
├── package.json               # 项目依赖配置
├── static/                    # 静态资源目录
│   └── logo/                  # 应用图标 (PWA Icon)
└── www/                       # 前端源代码目录
    ├── assets/
    │   ├── fonts/             # 图标字体文件
    │   ├── images/            # 图片资源 (Logo, 二维码等)
    │   ├── scripts/           # JS 脚本 (Bootstrap Bundle)
    │   └── style/             # CSS 样式文件
    ├── index.html             # 主页/考试入口
    ├── km3.html               # 考试模块页面
    ├── contact.html           # 联系我们页面
    └── profile.html           # 个人中心页面
```

## 快速开始

1. **环境准备**：
   - 安装 [Node.js](https://nodejs.org/)
   - 安装 [Android SDK](https://developer.android.com/studio#command-line-tools)
   - 全局安装 Cordova：`npm install -g cordova`

2. **构建 Android APK**：
   ```bash
   # 安装依赖
   npm install
   
   # 添加 Android 平台
   cordova platform add android
   
   # 构建 Release 包 (需配置签名)
   cordova build android --release
   ```

## 许可证

本项目遵循相应的开源或商业许可证（请查看源码根目录 LICENSE 文件）。