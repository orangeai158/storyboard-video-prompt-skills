---
name: orange-roaming-storyboard-prompt
description: Use this skill when the user wants to turn a short film idea, advertising concept, story project card, TVC concept, animation short, cyberpunk or wuxia concept, warm emotional short, or other video/storyboard brief into a nine-panel Image2 storyboard prompt, or when the user wants Seedance 2.0 image-to-video prompts based on a confirmed storyboard. Do not use for ordinary chat, research, article writing, coding, single-image illustration prompts, or non-storyboard image prompts without video or sequential storytelling needs.
---

# Orange Roaming Storyboard Prompt

## Purpose

Turn rough short-film, commercial, animation, or story concepts into:

1. A clean project card.
2. A continuous nine-panel Image2 storyboard prompt.
3. After storyboard confirmation, Seedance 2.0 image-to-video prompts for an approximately 15-second video.

Default output language is Chinese. Keep necessary camera terms in English when they are clearer, such as `slow push in`, `rack focus`, `match cut`, `hero shot`, `tracking shot`, and `4K cinematic quality`.

## Invocation Rules

Use this skill when the user asks for any of the following:

- 九宫格故事板, Image2 故事板提示词, TVC 广告故事板, 动漫短片分镜, 短片分镜.
- A video concept split into continuous scenes or shots.
- Consistent character, product, or environment prompts across storyboard panels.
- Seedance 2.0 image-to-video prompts based on a final storyboard.

Do not use this skill when the user only wants:

- A single still image prompt.
- A normal article, chat response, factual lookup, or code task.
- Generic image prompt optimization with no video, storyboard, or sequential narrative.

## Operating Mode

First identify the requested phase:

- **Image2 phase**: User wants a nine-panel storyboard or storyboard prompt.
- **Seedance phase**: User has a confirmed storyboard and wants video prompts.
- **Mixed phase**: User asks for both. Produce the Image2 storyboard first, then ask for confirmation before final Seedance prompts unless the user explicitly says to proceed directly.

If key details are missing, infer a tasteful default and mark it as an assumption. Ask a question only when the missing detail changes the core subject, brand/product, protagonist, or required format.

## Workflow

1. Normalize the project card:
   - 标题
   - 类型
   - 画幅比例
   - 主角/产品
   - 核心场景
   - 故事核心
   - 视觉风格
   - 情绪目标
   - 必须保持
   - 禁止出现
2. Build continuity anchors:
   - Character identity, clothing, age, silhouette, expression range.
   - Product appearance, material, color, logo visibility, placement.
   - World rules, location logic, lighting direction, time of day.
   - Recurring visual motif or emotional object when useful.
3. For Image2, create a nine-panel storyboard:
   - The nine panels must form a clear beginning, development, turn, climax, and ending.
   - Each panel should include subject, action, scene, composition, camera/lens feel, lighting, mood, and continuity notes.
   - Preserve the same protagonist/product/setting unless the story intentionally changes them.
   - Include a concise negative prompt section.
   - Use the template in `references/image2_storyboard_template.md` when detailed formatting is needed.
   - Use `references/storyboard_case_patterns.md` to choose the right narrative pattern for emotional shorts, TVCs, travel films, wuxia, cyberpunk, action comedy, or character boards.
   - Use `references/style_genre_rules.md` when the user asks for a specific visual genre or the concept implies one.
4. For Seedance, only after the storyboard is confirmed:
   - Generate prompts in storyboard order for an approximately 15-second video.
   - Include shot duration, camera movement, subject action, transition, sound/music suggestion, and negative constraints.
   - Use the template in `references/seedance_video_template.md` when detailed formatting is needed.
5. End with optional micro-adjustments:
   - Offer 2-4 focused tuning directions, such as more commercial, more cinematic, more emotional, more surreal, or more product-forward.

## Quality Bar

- The output must be directly usable as production prompt text, not only advice.
- Avoid vague labels like "高级感" unless translated into visible details.
- Do not let panel descriptions become isolated posters; every panel must advance the same story.
- Maintain visual consistency across panels by repeating the same anchor details.
- Keep prompts dense enough for generation, but avoid stuffing contradictory style references.
- If using brand/product content, keep the product visible at the important story beats without turning every frame into a hard sell.
- For Seedance, explicitly prevent animating the whole nine-grid image as one picture; the video must follow panel order.

## Output Shape

Use this default structure:

```markdown
## 1. 项目卡整理

## 2. Image2 故事板生成提示词
或
## 2. Seedance 2.0 视频制作提示词

## 3. 可选微调建议
```

When the user only asks for Seedance and provides no confirmed storyboard, first ask them to provide the final storyboard or offer to create the Image2 storyboard first.
