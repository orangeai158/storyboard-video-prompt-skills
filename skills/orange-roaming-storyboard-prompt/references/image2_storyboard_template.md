# Image2 Nine-Panel Storyboard Template

Use this reference when generating detailed Image2 storyboard prompts.

## Project Card Format

```markdown
## 1. 项目卡整理

- 标题：
- 类型：
- 画幅比例：
- 主角/产品：
- 核心场景：
- 故事核心：
- 视觉风格：
- 情绪目标：
- 必须保持：
- 禁止出现：
- 默认假设：
```

Only include `默认假设` when the user omitted important details and the skill inferred them.

## Storyboard Prompt Format

```markdown
## 2. Image2 故事板生成提示词

请生成一张九宫格故事板，整体为 [比例]，九个画面连续叙事，主角/产品/场景保持一致。

统一视觉设定：
[角色、产品、场景、光线、色彩、镜头质感、风格关键词、画质要求]

九宫格分镜：

1. [镜头名]
   画面：[主体 + 动作 + 场景]
   构图：[景别 + 视角 + 主体位置]
   镜头感：[lens/camera feel]
   光线与色彩：[lighting + palette]
   情绪：[emotion]
   连续性：[what must stay consistent]

2. ...

负面提示词：
[禁止元素、错误风格、角色不一致、产品变形、logo 错误、多余文字、低清晰度等]
```

## Nine-Panel Narrative Rhythm

Use this default rhythm unless the user's concept demands another structure:

1. Establishing shot: world, tone, protagonist/product appears.
2. Desire or problem: show what is missing, blocked, or desired.
3. First action: protagonist/product begins to change the situation.
4. Escalation: stakes rise, environment responds.
5. Turning point: emotional or visual midpoint.
6. Transformation: the key value or magic becomes visible.
7. Climax: strongest visual beat, `hero shot` if commercial.
8. Resolution: emotional payoff or proof of result.
9. Final image: memorable end frame, brand/product/story symbol.

## Consistency Anchors

Repeat the anchors in every panel where relevant:

- Character: age, face shape, hair, outfit, silhouette, signature prop.
- Product: exact shape, material, color, logo placement, scale, surface details.
- Environment: time of day, architecture, weather, color temperature.
- Style: rendering mode, film stock/camera feel, lighting behavior, texture.

## Negative Prompt Defaults

Use or adapt:

```text
角色身份不一致，服装变化过大，产品外形变形，logo 错误或乱码，多余文字，手指错误，脸部崩坏，画面低清晰度，过度磨皮，塑料质感，廉价广告海报感，风格混乱，九宫格之间色调断裂，主体比例异常，重复人物，错误透视。
```
