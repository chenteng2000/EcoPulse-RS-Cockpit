# Data Cockpit (数据驾驶舱)

基于 Vue 3 + Vite + TypeScript 构建的现代化企业级数据驾驶舱（Data Cockpit）项目。专为大屏数据可视化、实时业务监控与多维数据分析而设计。

## ✨ 特性

- ⚡️ **极速开发**: 基于 Vite 构建，提供极速的冷启动和 HMR (热更新)。
- 🛠️ **强类型**: 使用 TypeScript 编写，提供更好的代码提示和类型检查，提升项目稳定性。
- 📦 **基建完善**: 已配置绝对路径别名 (`@` -> `src`) 等开发提效功能。
- 📊 **大屏可视化**: 专为数据驾驶舱场景打造，预备集成 Apache ECharts / AntV，支持丰富的图表及动态动效展示。
- 📈 **实时展现**: 支持对接实时数据流（如 WebSocket），确保核心业务指标动态、实时更新。
- 🧩 **自适应布局**: 提供大屏适配方案，保证在不同分辨率及超宽比例屏幕终端上的完美呈现。

## 🚀 快速开始

### 环境要求

推荐使用 Node.js 18.x 或更高版本。

### 安装依赖

```bash
npm install
# 或者如果你使用 pnpm
pnpm install
```

### 启动开发服务器

```bash
npm run dev
# 或者
pnpm dev
```

### 构建生产版本

```bash
npm run build
# 或者
pnpm build
```

## 📁 核心目录结构

```text
├── src/
│   ├── assets/       # 静态资源
│   ├── components/   # 公共组件
│   ├── views/        # 页面 (路由视图)
│   ├── App.vue       # 根组件
│   └── main.ts       # 全局入口文件
├── vite.config.ts    # Vite 配置
└── package.json      # 项目元数据及依赖
```

## 📄 开源协议

本项目基于 MIT 协议开源。