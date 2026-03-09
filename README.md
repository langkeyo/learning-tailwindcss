# learning-tailwindcss

Tailwind CSS 学习项目仓库，按 `lesson-*` 目录拆分每节练习内容。

## 当前进度

- `lesson-01`：初始化练习（已创建目录）
- `lesson-02`：完成 Acme Rockets 页面基础结构与 Tailwind 样式编译
  - 包含响应式导航与页面分区（Hero / Rockets / Testimonials / Contact）
  - 已配置 Tailwind v3 编译链路
  - 已接入 Prettier + `prettier-plugin-tailwindcss`

## 目录结构

```text
lesson-02/
  src/
    input.css              # Tailwind 输入文件
  build/
    index.html             # 页面入口
    css/style.css          # Tailwind 编译产物
    img/*                  # 页面素材
  tailwind.config.js
  package.json
```

## 本地运行（lesson-02）

```bash
cd lesson-02
pnpm install
pnpm run tailwind
```

说明：

- `pnpm run tailwind` 会监听 `src/input.css` 并输出到 `build/css/style.css`
- `tailwind.config.js` 当前扫描范围为 `./build/*.html`

## 常用命令（lesson-02）

```bash
pnpm run tailwind
pnpm run prettier
```

## 版本说明

- Node 建议通过 Volta 管理
- 当前课程使用 `tailwindcss@3.x`（保留 `init` 与传统配置文件流程，适配多数入门教程）
