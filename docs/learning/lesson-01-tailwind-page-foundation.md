# Lesson 01: Tailwind 页面骨架与响应式导航

## Tempo Verdict
- 持平（首回合基线：2026-03-10 建立学习节奏，后续回合再比较快慢）

## Goal
- 读懂 `lesson-02/build/index.html` 的页面分层（`header` / `main` / `section`）。
- 能解释常见 Tailwind 工具类在本页里的作用（布局、间距、排版、颜色、响应式）。
- 在不看答案的情况下，独立完成一个“补全 Hero 区块”的练习。

## Context (Project + Business)
- 这是一个 Tailwind CSS 学习仓库，按 `lesson-*` 逐课推进。
- 当前 `lesson-02` 已具备 Acme Rockets 的基础页面和编译链路，核心是练会“快速搭页面 + 响应式调整”。
- 业务目标很简单：让用户快速理解品牌、产品（rockets）、评价和联系方式。

## Prerequisites
- 会运行：`cd lesson-02 && pnpm install && pnpm run tailwind`。
- 知道 HTML 基本结构和 class 属性。
- 愿意先自己动手，再对照检查点。

## Key Concepts
- `max-w-4xl mx-auto`：限制内容宽度并居中，避免超宽屏阅读困难。
- `flex` + `justify-between` + `items-center`：横向分布并垂直对齐。
- `sm:*`：从小屏断点开始生效，实现移动端优先。
- `dark:*`：暗色模式下替换颜色样式。
- `sticky top-0 z-10`：导航吸顶并保持层级在上方。

## Guided Steps (Read -> Think -> Do)
1. Read：通读 `lesson-02/build/index.html`，只看结构，不纠结每个 class。
2. Think：回答两个问题：
   - 为什么 `nav` 在小屏是 `hidden`，在 `sm` 以上又 `block`？
   - 为什么主内容容器和顶部容器都用了 `max-w-4xl mx-auto`？
3. Do：尝试给 Hero 区块补齐“右侧火箭图片 + 按钮组”结构（先自己写，不看现成教程）。

## Exercise A (Core)
- Task:
  - 在 `#hero` 内补充右侧图像区域，并加两个 CTA 按钮（例如“Explore Rockets”“Order Now”）。
- Constraints:
  - 不改 Tailwind 配置。
  - 保持移动端优先，小屏上下布局，大屏左右布局。
  - 颜色风格保持与头部一致（teal/indigo 体系）。
- Hints:
  - 图像区域可用 `sm:w-1/2` 与文字区域对称。
  - 按钮容器可以用 `flex gap-*`。
  - 大标题与按钮之间用 `mt-*` 拉开层次。
- Acceptance Criteria:
  - 小屏：标题在上、图或按钮在下，内容不拥挤。
  - `sm` 及以上：左右布局稳定，按钮不换行或换行也不破版。
  - 页面无明显水平滚动条。

## Exercise B (Stretch)
- Task:
  - 给顶部导航添加“当前区块高亮”的视觉效果（先做静态态，不做 JS 滚动监听）。
- Constraints:
  - 仅用 Tailwind 类，不引入额外 CSS 文件。
  - 不修改 HTML 语义结构（保留 `nav` + `a`）。
- Hints:
  - 可尝试 `font-semibold`、`underline`、`decoration-*`、`opacity-*` 组合。
- Acceptance Criteria:
  - 至少一个链接有“当前页”态。
  - 未激活链接与激活链接对比清晰。

## Checkpoints (Self-Review)
- 我能说清楚这 5 类工具：布局、间距、字号、颜色、响应式。
- 我能解释为什么 Tailwind 推荐“组合小类”而不是写长 CSS。
- 我能在 15 分钟内重构一个简化版 Hero。

## Common Pitfalls
- 把 `sm:` 理解反了（它是“到 sm 才生效”，不是“只在手机生效”）。
- 只追求桌面效果，忘了先保证移动端。
- `h-screen` 导致某些移动端可视高度表现不一致，后续课会讲替代策略。

## Glossary
- Utility-first：通过小而单一职责的 class 组合样式。
- Breakpoint：响应式断点，例如 `sm`, `md`, `lg`。
- CTA：Call To Action，引导用户行动的按钮/链接。

## Next Lesson Preview
- 下一课：组件化思维入门。把“按钮”“卡片”“section 标题”抽成可复用片段，并练习命名规范。
