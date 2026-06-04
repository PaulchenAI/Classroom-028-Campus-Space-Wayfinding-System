# Classroom 028 Campus Space Wayfinding System

校园 028 教室导视单页应用，使用 `Vite + React + TypeScript` 构建。

## 本地运行

前置条件：`Node.js 20+`

1. 安装依赖
   `npm install`
2. 启动开发环境
   `npm run dev`
3. 本地构建
   `npm run build`

## GitHub Pages 部署

仓库地址：
`https://github.com/PaulchenAI/Classroom-028-Campus-Space-Wayfinding-System`

项目已经按 GitHub Pages 子路径部署做了配置：
- 生产环境 `base` 为 `/Classroom-028-Campus-Space-Wayfinding-System/`
- 推送到 `main` 后，GitHub Actions 会自动构建并发布 `dist/`

首次启用时需要在 GitHub 仓库设置里确认：
1. 打开 `Settings -> Pages`
2. `Source` 选择 `GitHub Actions`

发布成功后，默认访问地址为：
`https://paulchenai.github.io/Classroom-028-Campus-Space-Wayfinding-System/`

## 说明

- `ConsoleApp1/` 是独立的 .NET 控制台项目，不会部署到 GitHub Pages
- GitHub Pages 只会托管前端静态构建产物 `dist/`
