# Seedance 2.0 Image-To-Video Template

Use this reference when generating Seedance 2.0 prompts from a confirmed storyboard.

## Preconditions

Seedance prompts should be generated from the final confirmed storyboard. If the user has not confirmed a storyboard, ask for the final storyboard or offer to create the Image2 storyboard first.

## Output Format

```markdown
## 2. Seedance 2.0 视频制作提示词

视频总设定：
- 时长：约 15 秒
- 比例：
- 主角/产品一致性：
- 视觉风格：
- 节奏：
- 音乐/声音方向：
- 统一负面约束：

分镜视频提示词：

镜头 1 / 0:00-0:02
- 参考图：第 1 格故事板
- 画面动作：
- 镜头运动：
- 转场：
- 声音：
- Seedance 提示词：

镜头 2 / 0:02-0:04
...
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

## Negative Constraint Defaults

Use or adapt:

```text
保持主角身份和服装一致，保持产品形状、颜色和 logo 位置一致，避免面部漂移，避免肢体变形，避免产品融化或拉伸，避免镜头突然跳切，避免背景风格突变，避免多余文字和错误字幕，避免低清晰度、闪烁、过度运动模糊和不自然补帧。
```
