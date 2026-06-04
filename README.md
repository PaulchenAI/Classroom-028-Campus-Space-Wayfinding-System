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

## 更换仓库后重新部署

如果项目迁移到新的 GitHub 仓库，可以重新部署到 GitHub Pages，但不要只改远程仓库地址，还需要同步检查前端发布路径配置。

建议按下面顺序处理：

1. 修改 Git 远程仓库地址并推送代码
2. 如果新仓库名发生变化，修改 [vite.config.ts](/Users/cm/Projects/Classroom_028_Campus_Space_Wayfinding_System/vite.config.ts) 中生产环境的 `base`
3. 更新本 README 中的仓库地址和 GitHub Pages 访问地址
4. 在新仓库的 `Settings -> Pages` 中确认 `Source` 为 `GitHub Actions`
5. 推送到 `main`，等待 GitHub Actions 重新发布

说明：
- 如果只是更换仓库账号，但仓库名保持不变，`base` 通常不用改
- 如果仓库名变了，`base` 必须跟着改，否则页面静态资源路径会错误

## 说明

- `ConsoleApp1/` 是独立的 .NET 控制台项目，不会部署到 GitHub Pages
- GitHub Pages 只会托管前端静态构建产物 `dist/`
