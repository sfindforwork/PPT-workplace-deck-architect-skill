# Workplace visual language

The default style is restrained workplace communication: clear structure, strong alignment, and enough visual interest to distinguish relationships without competing with the content. This is a decision framework, not a fixed palette or a single personal-deck template.

## Choose the system by situation

Before selecting colors or components, identify the communication job, audience and source constraints.

| Situation | Visual priority | Good forms | Avoid |
|---|---|---|---|
| 述职 / 转正 / 个人复盘 | 证据、进展、个人能力与反思 | 固定章节索引、编辑型网格、编号、轻量时间线 | 过度品牌化、没有证据的口号 |
| 项目计划 / 产品方案 | 范围、系统关系、阶段与决策 | 系统图、流程、阶段轴、边界表、责任映射 | 把每个要点做成广告卡片 |
| 调研 / 数据复盘 | 数据可信度、对比和结论依据 | 指标、对比矩阵、标注证据、来源说明 | 用大数字替代分析 |
| 培训 / 使用指南 | 可跟随、可查找、可操作 | 步骤导航、示例、进度标记、目录锚点 | 只追求视觉冲击 |
| 品牌 / 宣传 / 活动 | 记忆点、情绪和传播性 | 强图像、品牌色、动效、节奏变化 | 在非宣传场景里套用营销风格 |

述职项目中形成的米白底、蓝色结构色、橙色强调色、右侧章节索引等，只在用户明确要求或内容确实匹配时复用。它不是所有 PPT 或 H5 的默认外观。

H5 比 PPT 更容易承载交互，但交互必须帮助理解：目录跳转、滚动揭示、图片高清查看、局部展开、轻量过渡和演讲者模式都可以使用；漂浮装饰、无意义粒子、自动播放大动画和“看起来像广告”的动效默认不使用。

Fixed-stage H5 页面在宽屏上可能出现左右留白；让外层画布背景跟随当前页面的深浅色状态，避免深色章节页被浅色边条切开。页面切换使用短促、克制的整体淡入 / 轻位移即可，不要让章节封面和正文在切换时突然跳变。

## Global system

Start with a small, reusable design system. The personal default palette is:

```text
paper  #f7f3ed   quiet warm background
ink    #202228   primary text
muted  #76716b   secondary text
blue   #2859d5   structure, navigation, active information
red    #ed6b52   current state, emphasis, or correction
line   #d9d1c5   separators and inactive structure
```

The user may override these values, but do not introduce a new accent color on one page without a system-wide reason.

Keep these invariants stable within one deliverable:

- main left and right gutters;
- title and kicker baseline;
- top marker and page counter;
- footer label and page number;
- chapter navigation location and active state;
- image frame treatment and lightbox behavior;
- heading sizes and spacing between hierarchy levels.

## Workplace structure, not advertising composition

Prefer when they match the situation:

- a quiet cover with title, name, and one purposeful visual;
- a contents page that exposes the whole route;
- chapter covers that clearly separate units;
- fixed section navigation that answers “where am I?”;
- a restrained grid, rules, numbers, and short labels;
- visible evidence and explicit relationships.

Avoid by default:

- a marketing-style hero slogan;
- oversized decorative type that pushes content away;
- gradients, floating pills, random blobs, or decorative color blocks;
- a row of generic cards used only to fill space;
- unrelated illustrations placed because a corner is empty;
- too many circular path diagrams;
- repeated “summary” sentences that are not in the source.

## Page composition

Use a page anatomy that can be reused:

```text
top marker / page counter
chapter navigation + page title
main relationship or content structure
evidence / image / supporting detail
footer / page number
```

The title must establish the page before the viewer encounters the component. If navigation or a top bar is removed, reclaim the released space intentionally; never leave a stranded blank row.

For a deck with several chapters, use an index rail rather than repeating a long chapter label on every page. Choose its mode from the communication job: a reading-first, long, or content-dense deck should use a detailed side rail with full chapter names plus human-readable page titles; a short, speaker-led deck may use a quiet bottom rail with chapter labels only. Choose the side by visual weight, not by habit: use the right when the title and main reading structure are left-heavy and the right side has a stable gutter; use the left when the right side contains imagery or diagrams; use the bottom only when neither side can be reserved without squeezing the content. A side rail needs real reserved space and must not overlay body text or visuals. Keep a right rail visually quiet: it should not become an opaque panel or a full-height divider; a short header rule, indentation, and small active markers are enough to make the route legible. A horizontal index is not a process diagram: do not run one continuous line through the labels. Use hierarchy, indentation, separated text units, subtle dividers or whitespace, and one restrained accent state for the current chapter / page. Keep it clickable in H5, hide it on cover / contents / closing pages when it adds noise, reclaim the hidden rail's gutter on those pages, and do not use arbitrary alternating colors to simulate hierarchy.

## Components should carry meaning

- Thin lines separate levels or connect stages.
- Numbers show order or provide an index; they should not be decorative labels.
- Blue indicates structure, active navigation, or a highlighted ability.
- Red indicates a current state, a key correction, or a meaningful emphasis.
- A border or color block needs to define a real group; otherwise use whitespace and a rule.
- A repeated component should have the same position, scale, and semantics on every page.
- Color should follow the information relationship: keep one accent for a collection without internal semantic differences; introduce multiple accents only for meaningful categories, sources, roles, statuses, or phases. Avoid alternating colors as decoration.

When a page needs a visual form, choose it from the relationship between the contents. A timeline is not a universal solution, and a circular diagram is not a synonym for “process”. A component that looked good in a述职 deck must be re-justified for a project plan, product proposal, research report or guide.

## Density and spacing

Do not solve overflow by shrinking everything until it becomes unreadable. In order:

1. remove duplicated labels or repeated explanations;
2. separate the main claim from supporting evidence;
3. reduce unnecessary vertical padding;
4. adjust the ratio between text and image columns;
5. shorten only source-faithful wording;
6. change font size as a last resort.

Whitespace is useful when it establishes hierarchy. It is a defect when it is caused by removing a component, leaving an unused grid track, or placing the content too low.
