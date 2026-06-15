# Nine-Panel Storyboard Template

Use this reference when generating detailed storyboard prompts. This template is not limited to Image2 — it applies to any image generation tool or style the user specifies.

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
## 2. 故事板生成提示词

创建一张专业电影级九宫格故事板，用于 [项目类型]《[标题]》的前期制作。

布局：[比例] 横版九宫格故事板，3x3 grid，正好 9 格。每格是独立清晰的分镜，干净边框，阅读顺序从左到右、从上到下。整体是连续叙事 storyboard，不是九张独立海报，不是杂乱拼贴。可以保留极小的 1-9 分镜编号。

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

## Lock Sections

Use the lock sections that fit the project:

- `【核心创意】`: one paragraph describing the story, emotional turn, or commercial idea.
- `【角色锁定】`: protagonist identity, age, hair, outfit, expression rules, recurring props.
- `【产品锁定】`: product shape, material, color, logo/text policy, what must never change.
- `【场景锁定】`: where each panel happens, what can change, what must stay fixed.
- `【视觉风格】`: concrete lighting, color, camera, texture, and genre terms.
- `【参考优先级】`: when uploaded references exist, state what each reference controls.

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

## Reference Priority Pattern

When the user provides reference images or a confirmed project card, state priority explicitly:

```text
参考优先级：如果上传了角色、产品、动物、交通工具、环境或故事板参考图，请严格使用参考图控制外观、比例、服装、颜色、道具和场景关系。
本故事板控制：分镜顺序、动作逻辑、镜头构图、空间连续性、光线方向、情绪节奏和转场逻辑。
```

## Negative Prompt Defaults

Use or adapt:

```text
角色身份不一致，服装变化过大，产品外形变形，logo 错误或乱码，多余文字，手指错误，脸部崩坏，画面低清晰度，过度磨皮，塑料质感，廉价广告海报感，风格混乱，九宫格之间色调断裂，主体比例异常，重复人物，错误透视。
```
