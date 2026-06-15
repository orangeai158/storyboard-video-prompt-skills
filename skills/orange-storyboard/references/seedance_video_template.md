# Seedance 2.0 Image-To-Video Template

Use this reference when generating Seedance 2.0 prompts from a confirmed storyboard.

## Preconditions

Seedance prompts should be generated from a storyboard provided by the user. The storyboard can be in any format: an Image2 nine-panel grid, a hand-drawn scan, a text description of panels, or any other sequential panel format. If the user has not provided any storyboard, ask them to provide one or offer to create the Image2 storyboard first.

When the source is a nine-panel grid image, never tell Seedance to animate the full sheet as a single image. The prompt must instruct that the video be generated panel by panel in order. When the source is a text or other non-image storyboard, derive the visual reference from the panel descriptions instead.

## Output Format

All output must be in Chinese. Camera movement terms may remain in English when they are clearer (e.g. slow push in, rack focus, tracking shot, hero shot, locked-off). The Seedance prompt text field must also be written in Chinese, not English.

When the storyboard panels are not numbered, do not reference panels by position (左上、中上 etc.). Instead, number them 镜头1–镜头9 sequentially and identify each by its content (e.g. "门口全景建立镜头" or "猫靠近手指特写").

Output must not exceed 2000 Chinese characters in total.

```markdown
## 2. 图生视频提示词

使用上传的最终九宫格故事板作为唯一主要视觉参考。不要整图生成，不要把九宫格当成一张完整图片来动画化，必须按第 1 格到第 9 格的分镜顺序生成连续视频。

视频总设定：
- 时长：约 15 秒
- 比例：
- 主角/产品一致性：
- 视觉风格：
- 节奏：
- 音乐/声音方向：
- 统一负面约束：

分镜提示词：

镜头 1 / 0:00-0:02 ｜ [内容简述]
- 画面：
- 镜头：
- 转场：
- 声音：
- 动作：

镜头 2 / 0:02-0:03.5 ｜ [内容简述]
...
```

## Opening Lock Formula

Use this pattern at the beginning of Seedance output:

```text
REFERENCE: 使用上传的最终九宫格故事板作为主要视觉参考。严格保持 [角色/产品/场景/光线/故事顺序] 一致。不要整图生成，不要把九宫格当作一张图动画化，必须按照第 1 格到第 9 格分镜顺序生成连续视频。不要添加额外角色。不要改变剧情。不要改变服装、道具、产品外观和场景关系。不要添加字幕、logo、UI、水印。不要出现文字和数字。
STYLE: [visual style, lighting, texture, genre]
CAMERA RULES: [pace, motion intensity, emotional rhythm, what to avoid]
TIMESTAMPED SEQUENCE:
```

## Fifteen-Second Timing

Default timing for nine storyboard panels:

- Shot 1: 0:00-0:02
- Shot 2: 0:02-0:03.5
- Shot 3: 0:03.5-0:05
- Shot 4: 0:05-0:06.5
- Shot 5: 0:06.5-0:08.5
- Shot 6: 0:08.5-0:10
- Shot 7: 0:10-0:12
- Shot 8: 0:12-0:13.5
- Shot 9: 0:13.5-0:15

Adjust timing if the user requests another duration.

## Camera Language

Use specific motion language:

- `slow push in`: emotional reveal, product attraction, intimacy.
- `tracking shot`: follows movement through a space.
- `rack focus`: shifts attention between subject and product/detail.
- `match cut`: links similar shapes or actions across shots.
- `hero shot`: final product or protagonist payoff.
- `handheld subtle motion`: realism and urgency.
- `locked-off symmetrical frame`: ritual, calm, premium control.

## Seedance Prompt Requirements

Each shot prompt should include:

- Starting frame based on storyboard panel.
- What moves and what stays stable.
- Camera movement and speed.
- Subject action.
- Environmental motion such as light, smoke, rain, fabric, particles, or crowd flow.
- Transition to the next shot.
- Negative constraints to prevent deformation and identity drift.

Each shot should be written as a production instruction, not a short caption. Include visible motion, environmental motion, sound, rhythm, and transition.

## Negative Constraint Defaults

Use or adapt:

```text
保持主角身份和服装一致，保持产品形状、颜色和 logo 位置一致，避免面部漂移，避免肢体变形，避免产品融化或拉伸，避免镜头突然跳切，避免背景风格突变，避免多余文字和错误字幕，避免低清晰度、闪烁、过度运动模糊和不自然补帧。
```
