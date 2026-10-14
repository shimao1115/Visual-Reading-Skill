# Visual Reading Skill｜全文视觉陪读

将长篇文章、评论、经典和教学阅读材料，制作成以**原文阅读为中心**的单文件 HTML 课堂课件。

**核心方法：Source + Interpretation**

- 左侧 Source：按原始顺序完整阅读正文，不用摘要取代文本。
- 右侧 Interpretation：根据当前段落同步呈现图解、证据、背景、对比或追问；右侧不替代原文。
- 使用滚动驱动阅读节拍（step）和视觉场景（scene），让教师可随时停下来讲解与回滚。
- 先读全文再构思视觉，不预设页数、step 数量或固定配图模板。

## 仓库内容

- [SKILL.md](SKILL.md)：可供 Codex 等兼容 Agent Skills 的工具阅读和执行的规范。
- [assets/visual-reading-demo.html](assets/visual-reading-demo.html)：原创占位文本的最小交互演示，展示双栏 sticky 舞台、滚动同步和回滚；**不是**可用于验证全文覆盖的历史课件。

## 给 Codex 使用

可以直接把本仓库地址发给 Codex，并告诉它：

> 请从 https://github.com/shimao1115/Visual-Reading-Skill 安装或读取 `visual-reading` Skill，然后按 SKILL.md 的要求，使用我提供的文章**完整正文**制作单文件 HTML 全文视觉陪读课件。请真实检查 1920×1080 投影效果、全文覆盖和从头到底再回滚的场景同步。

如需在本机长期复用，Codex 可将本仓库克隆到其用户级技能目录（如 `~/.agents/skills/visual-reading`），确认根目录有 `SKILL.md` 后再加载。**仅发送仓库网址不代表自动安装**；首次请让 Codex 明确读取或安装。

## 来源与授权边界

方法提炼自 2026-09-23《思考正在成为一种奢侈品》课堂视觉阅读成品及其制作提示词。旧成品包含第三方新闻文章的课堂改写正文，因此**不在公开仓库发布旧成品全文**；本仓库演示采用原创占位材料，代码结构可以参考，实际视觉应依据新文章重新设计。

使用时请提供有权使用的完整文本，并清晰标注原文、译文、改写或节选；公开分享成品前请检查正文、照片、数据等资源的版权和引用边界。

## 设计态度

**Trust the capability, verify the outcome.**

本 Skill 固定产品目标、证据边界与验收，不把 AI 创造视觉场景的过程硬编码成一棵规则树。单文件 HTML 优先；不为课堂课件引入不必要的 framework、pipeline 或 Agent 架构。
