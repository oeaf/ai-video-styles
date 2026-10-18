# animate

https://github.com/cth9191/animate · 790 star · MIT · 2026-10-04 创建（评估时 10 commits，较新）

## 一句话

7 种内置风格 + **按你的参考图定制新画风**：故事、试看、分镜三步都先给你确认，通过了才开始烧时间做动画。

## 怎么玩

- 安装：`/plugin marketplace add cth9191/animate` / `/plugin install animate@animate`
- 用法：`/animate a 45-second history of the bicycle, cut paper`，或 `/animate a short about our API in the style of these screenshots: ./refs/`
- 流程：问卷 → 故事确认（beat 表）→ 试看确认（2–4 张全尺寸风格帧）→ 分镜确认（逐格关键帧）→ 制作 → 交付
- 自带配音（ElevenLabs 或自己录音）、节拍映射音乐、真实产品截图植入、9:16/1:1/4:5/16:9 多画幅一次输出

## 7 种内置风格

剪纸（cut paper）、素描（crosshatch）、孔版印刷（riso）、素描本（sketchbook）、数学解说（math，manim 风）、像素（pixel）、等距插画（isometric）

## 适合谁

- 有参考图/参考视频，想复刻某种画风的人：它会测量调色板、线条、质感、运动节奏，画出对比帧给你确认
- 产品宣传：能把真实产品截图放进动画里
- 数学/技术解说：math 风格对标 manim

## 注意

- 需要 Claude Code、Node 18+、Playwright + Chromium、ffmpeg
- 仓库较新（2026-10-04），长期维护状态待观察
