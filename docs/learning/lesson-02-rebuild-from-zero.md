# Lesson 02: 从抄写到重建（完整带练版）

## Tempo Verdict
- 进步（你主动暴露卡点并请求重建训练，这比继续机械抄写更高级）

## Goal
- 建立“删光也能写回来”的能力，而不是记住某一版代码。
- 学会把页面拆成可重建的 4 层：结构层、布局层、视觉层、响应式层。
- 在 45~60 分钟内独立重建当前 `lesson-02` 的核心页面骨架。

## Context (Project + Business)
- 你当前项目对应 Dave Gray 的 Tailwind 入门实战。
- 真正能力不是“照着敲完”，而是离开视频后仍能把页面搭回来。
- 所以训练目标是：从结果导向切换为“流程导向”。

## Prerequisites
- 能运行 `cd lesson-02 && pnpm run tailwind`。
- 允许自己先写出 70 分版本，再迭代到更接近教程效果。

## Key Concepts
- 结构层：先写语义标签（`header/main/section/article/nav`）。
- 布局层：只处理 `flex/grid/width/max-w/mx-auto/gap`。
- 视觉层：再补颜色、字号、间距、圆角、阴影。
- 响应式层：最后补 `sm/md/lg`，避免一开始就被断点打乱。

## Guided Steps (Read -> Think -> Do)
1. Read：先看最终页面，只记“区块清单”，不记 class。
2. Think：每个区块只回答两件事：
   - 它是横排还是竖排？
   - 它在小屏和大屏分别怎么变？
3. Do：按下面“重建脚本”执行，不允许跳步。

## Exercise A (Core) - 45 分钟重建脚本
- Task:
  - 把 `lesson-02/build/index.html` 备份后清空主体内容，从 0 重建到可用版本。
- Constraints:
  - 每一轮只改一层，不混改。
  - 每完成一层就在浏览器检查一次。
- Hints:
  - 第 1 轮（10 分钟）：只写结构，不加任何样式类。
  - 第 2 轮（15 分钟）：只加布局类（容器、flex、宽度、对齐、间距）。
  - 第 3 轮（10 分钟）：加视觉类（颜色、字号、粗细）。
  - 第 4 轮（10 分钟）：加 `sm:*` 和 `dark:*`。
- Acceptance Criteria:
  - 页面区块齐全：`Header + Hero + 基础导航`。
  - 小屏可读、大屏不散，且没有明显横向滚动。
  - 你能口述每个主要 class 的作用，而不只是“看起来对”。

## Exercise B (Stretch) - 反向记忆训练
- Task:
  - 关掉教程视频，5 分钟内写出你记得的 Hero 区块；再对照修正。
- Constraints:
  - 不复制粘贴旧代码。
  - 只允许参考你自己写的“区块清单”。
- Hints:
  - 忘了类名就先写语义和布局，类名后补。
- Acceptance Criteria:
  - 第一版能跑起来。
  - 第二版比第一版结构更清晰、类更有组织。

## Checkpoints (Self-Review)
- 我是不是先搭结构，再做样式？
- 我是不是能解释 class 作用，而不是背字符串？
- 我是不是每 10~15 分钟就完成一个可运行小版本？

## Common Pitfalls
- 一上来追求 100% 还原，导致卡死。
- 看到某个 class 忘了就停住，不继续。
- 布局和视觉混着改，自己也搞不清错在哪。

## Glossary
- 重建：不看原代码，按流程把页面再次搭出来。
- 区块清单：页面的大模块目录，不含具体 class。
- 70 分版本：先可用，再迭代，不追求一步到位。

## Next Lesson Preview
- 下一课：导航与移动端菜单的交互重建（按钮状态、可访问性、显示/隐藏逻辑）。
