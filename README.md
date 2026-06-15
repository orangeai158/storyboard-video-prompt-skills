# 橘子漫游的故事板提示词

这是一个 Codex skill，用于把短片创意、广告概念或故事项目卡扩写成可直接用于 Image2 的九宫格故事板提示词，并在故事板确认后生成 Seedance 2.0 图生视频提示词。

## Skill

- Skill name: `orange-roaming-storyboard-prompt`
- Install path: `skills/orange-roaming-storyboard-prompt`
- Explicit invocation: `$orange-roaming-storyboard-prompt`

## 适合场景

- 九宫格故事板
- Image2 故事板提示词
- TVC 广告故事板
- 动漫短片分镜
- 武侠、赛博朋克、温馨短片分镜
- 基于最终故事板生成 Seedance 2.0 图生视频提示词

## 示例调用

```text
$orange-roaming-storyboard-prompt
帮我把这个短片创意拆成 Image2 九宫格故事板提示词：
一个小男孩在雨后的旧街道捡到一只会发光的纸船，跟着它走到河边，发现纸船来自多年后的自己。
```

```text
帮我做一个高端香水 TVC 广告故事板，16:9，九宫格，风格要像欧洲清晨古堡花园。
```

```text
基于这个最终九宫格故事板，生成 Seedance 2.0 图生视频提示词。视频 15 秒，必须按第 1 格到第 9 格顺序生成，不要把九宫格整图动画化。
```

## 输出内容

默认输出中文，必要的专业镜头词会保留英文，例如 `slow push in`、`rack focus`、`match cut`、`hero shot`、`tracking shot`。

输出通常包括：

1. 项目卡整理
2. Image2 故事板生成提示词或 Seedance 2.0 视频制作提示词
3. 可选微调建议
