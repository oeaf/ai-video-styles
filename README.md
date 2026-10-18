# AI 视频风格选型手册

> ⭐ **Support This Project**
>
> [![GitHub stars](https://img.shields.io/github/stars/oeaf/ai-video-styles?style=social)](https://github.com/oeaf/ai-video-styles)
> [![GitHub forks](https://img.shields.io/github/forks/oeaf/ai-video-styles?style=social)](https://github.com/oeaf/ai-video-styles)
> [![GitHub issues](https://img.shields.io/github/issues/oeaf/ai-video-styles)](https://github.com/oeaf/ai-video-styles/issues)
>
> 如果这个项目对你有用，欢迎点个 ⭐ Star！你的支持是我持续更新的动力。

5 个 AI 视频风格工具的归类选型手册。它们走的是同一条技术路线——**Claude Opus 5.5 写代码做视频**（Canvas / WebGL 逐帧渲染 + ffmpeg 合成，不用视频生成模型，不用实拍素材）——但产品形态各不相同：风格库、风格探索、定制画风、单风格深耕。

逐个写进技能库又乱又重复，所以归到这一个仓库：**对比表 + 决策树 + 每家一页评估**。

## 对比总表（2026-10-18 评估）

| 工具 | 定位 | 风格 | 工作流 | Star | 协议 |
|---|---|---|---|---|---|
| [lemo-opuscar](tools/lemo-opuscar.md) | 影片风格库 | 51 种（水墨、皮影、浮世绘、像素、实证影像…），每种带一支纯代码样片 | 选风格→讲故事→可选分镜确认→成片（约 30–60 分钟） | 2894 | MIT |
| [huashu-art-motion](tools/huashu-art-motion.md) | 艺术风格 + 解说动画 | 35 种艺术风格，白板 / Vox / 3Blue1Brown 解说语法 | 代码绘制，可按口播参数渲染片段 | 已收录并安装 | — |
| [animate](tools/animate.md) | 定制画风 | 7 种内置（剪纸、素描、像素、等距插画、数学解说…）+ 按参考图配新画风 | 故事→试看→分镜，三步确认后再开工 | 790 | MIT |
| [xilo-opus-video](tools/xilo-opus-video.md) | 风格探索 | 不限：先给 3 个差别大的方案，每个带预览 | 3 方案→预览→确认→写 brief→逐镜制作 | 167 | MIT |
| [opus-video-skills](tools/opus-video-skills.md) | 单风格深耕 | 2 种：水彩手绘动画、动态文字 | 一个 skill 一种风格，即装即用 | 218 | MIT |

## 决策树：我该用哪个

```
有明确想要的风格？
├─ 是 → 风格库型：lemo-opuscar（51 种随便挑，每种有样片）
│         解说/知识类 → huashu-art-motion（解说动画语法）或 animate（math 风格）
├─ 没想法，想先看效果再定？
│       → xilo-opus-video（3 个差异方案带预览，选中再做）
├─ 有参考图，想复刻某种画风？
│       → animate（按参考图配新画风，分镜先确认）
└─ 做歌词 MV / 个人作品集？
        → opus-video-skills（水彩手绘 / 动态文字，单点做深）
```

## 每家一页

- [lemo-opuscar](tools/lemo-opuscar.md) —— 51 种影片风格库，每种带样片
- [huashu-art-motion](tools/huashu-art-motion.md) —— 35 种艺术风格 + 解说动画（已安装）
- [animate](tools/animate.md) —— 7 种内置 + 参考图定制新画风
- [xilo-opus-video](tools/xilo-opus-video.md) —— 3 方案预览式风格探索
- [opus-video-skills](tools/opus-video-skills.md) —— 水彩手绘 / 动态文字单风格

## 共同前提

- 都需要 Claude Code + Node + ffmpeg + Playwright/Chromium（各家 README 有具体版本要求）
- 成片是代码逐帧渲染的，**不适合**写实画面、剪辑现成素材、加字幕这类需求
- 评估日期 2026-10-18，star 数会变，选型时以仓库当前状态为准

## License

MIT
