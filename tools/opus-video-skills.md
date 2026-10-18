# opus-video-skills

https://github.com/tuzhechen2005/opus-video-skills · 218 star · MIT（README 声明）· 2026-09-26 创建

## 一句话

**一个 skill 一种风格**，单点做深：水彩手绘动画、动态文字，各自独立安装。

## 两个 skill

| skill | 风格 | 典型用途 |
|---|---|---|
| painted-animation | 水彩 + 水墨卡通，角色会表演 | 动画短片、MV、歌词 MV（带卡拉OK逐字字幕） |
| kinetic-reel | 动态排印：压缩展示字体 + HUD 微字 + WebGL 层 | 作品集、showreel、产品介绍 |

- 示例：31 秒陶喆《小镇姑娘》歌词 MV；84 秒 "Work Reel '26" 作品集
- 每帧都是时间的纯函数，headless Chrome 渲染 + ffmpeg 编码；音乐节拍实测后卡点

## 怎么玩

- 安装（二选一或都装）：`/plugin marketplace add tuzhechen2005/opus-video-skills`，然后 `/plugin install painted-animation@opus-video-skills`
- 用法：直接描述，"Make a 15-second video of Clawd trying to catch a butterfly"，skill 自动匹配或按名调用
- 每个 skill 出分镜→逐镜制作→审片→成品 MP4 写到 `out/`

## 适合谁

- 做歌词 MV、音乐视频的人（painted-animation 卡拉OK字幕是现成的）
- 做个人作品集/showreel 的人（kinetic-reel）
- 只想要一种风格、装完即用的人

## 注意

- 需要 Claude Opus 5.5、Node、Chrome、ffmpeg
- 风格只有 2 种，想要别的风格去看 lemo-opuscar / animate
