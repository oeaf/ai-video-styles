# xilo-opus-video

https://github.com/Kianzzz/xilo-opus-video · 167 star · MIT · 2026-09-28 创建（中文 README）

## 一句话

**风格探索型**：没想好要什么风格？它先给你 3 个差别很大的方案、每个带预览，你挑中一个它再开工。

## 怎么玩

- 安装：Claude Code 里说"帮我安装这个 Skill：https://github.com/Kianzzz/xilo-opus-video"，或 `npx skills add Kianzzz/xilo-opus-video`
- 流程：说需求（一句话/一篇文章/一个产品网址/一条参考视频都行）→ 3 个方案（风格、技术组合、分镜概括、声音、预计渲染时间）→ 每个方案一张关键帧或 2–4 秒小样 → 你确认 → 写成 `brief.md`（可复用的结构化提示词）→ 逐镜制作、自检 → 成片 MP4
- 技术栈：Canvas / HTML·CSS·SVG / WebGL 着色器 / Three.js / Remotion / HyperFrames / Manim，配乐代码合成

## 适合谁

- 不知道要什么风格、想先看效果再定的人
- 产品宣传片、知识讲解、像素/复古/手绘/界面动效类短片
- 照着参考视频的结构和手法做一条自己的
- 有视频模型生成的绿幕人物，想用代码搭场景加大字动效

## 不适合

- 直接生成写实画面（需要视频模型，它只做代码层）
- 在剪映/Premiere/AE 里剪辑现成素材、加字幕

## 注意

- star 最少（167），社区验证最少，但流程设计最完整（brief.md 可复用是亮点）
- 需要 Python 3.9+、playwright、FFmpeg、Chromium
