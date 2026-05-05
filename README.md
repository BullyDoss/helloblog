# Hello Blog

一个基于 Vue 3 + Express + MySQL 的全栈博客系统。

## 技术栈

### 后端
- Node.js + Express
- MySQL 数据库
- JWT 认证
- 图片上传 (Multer)
- CORS 跨域支持

### 前端
- Vue 3
- Vue Router
- Vite
- Axios
- Markdown 渲染

## 项目结构

```
.
├── blog-backend/      # 后端服务
│   ├── index.js       # 主入口文件
│   ├── create-admin.js # 管理员初始化脚本
│   └── uploads/       # 图片上传目录
└── blog-frontend/     # 前端应用
    └── src/
        ├── views/     # 页面组件
        ├── components/ # 公共组件
        ├── router/    # 路由配置
        └── utils/     # 工具函数
```

## 快速开始

### 后端

1. 安装依赖
```bash
cd blog-backend
npm install
```

2. 配置数据库

创建 `.env` 文件：
```env
MYSQL_HOST=localhost
MYSQL_USER=root
MYSQL_PASSWORD=your_password
MYSQL_DATABASE=blog_db
JWT_SECRET=your-secret-key
PORT=3000
```

3. 创建数据库表并初始化管理员
```bash
node create-admin.js
```

4. 启动服务
```bash
npm run dev
```

### 前端

1. 安装依赖
```bash
cd blog-frontend
npm install
```

2. 启动开发服务器
```bash
npm run dev
```

## 功能特性

- 用户注册与登录
- JWT 身份验证
- 文章发布与编辑
- Markdown 内容支持
- 图片上传功能
- 响应式设计

## License

ISC
