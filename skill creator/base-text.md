# 角色资产展示板字体规范 (base-text.md)
## Character Presentation Board Typography Specification

展示板的高奢大刊感，核心在于**全板字体的极简统一**。提示词中无需繁琐约束，只需严格定义以下三套字体：

---

### 1. 核心字体三件套 (The Typographic Triad)

1. **结构与西文标题 (Global Western & UI Headers)**
   - **字体定义**：`High-contrast editorial Didone serif (all uppercase)`
   - **作用范围**：顶部双行大标、右上角元数据、8 大容器标题 (`BASIC INFORMATION`, `MODEL SHEET`, `EXPRESSIONS` 等)、三视图标签 (`FRONT`, `SIDE`, `BACK`) 及工业色卡 HEX 码。
   - **视觉效果**：类似《Vogue》大刊的高反差锐利衬线，全板统一，自带高级呼吸感。

2. **中文正文与诗意引言 (Chinese Text & Lore)**
   - **字体定义**：`Airy tracked Songti (spaced Chinese characters)`
   - **作用范围**：顶部主标题下方的设计引言、人物小传段落、核心关键词。
   - **视觉效果**：字距舒展拉开的典雅宋体，清透不凝滞。

3. **艺术签名 (Signature Script)**
   - **字体定义**：`Flowing cursive handwritten script in black ink`
   - **作用范围**：右下角专属签名 `[CharacterName] ♡` 及下衬宣言。
   - **视觉效果**：极度优美的黑色连笔花体手写，增添画龙点睛的个人印记。

---

### 2. 提示词标准单句注入模板 (Prompt Snippet)

在向大模型交付英文提示词时，直接注入以下简练描述即可锁定全局版式：

```text
Typography: global UI titles and container headers strictly rendered in high-contrast editorial Didone serif in all uppercase; Chinese quotes and lore in elegant airy tracked Songti; character signature in flowing cursive handwritten script in black ink.
```

---

### 3. 三条防翻车硬规避 (Key Safeguards)

- **顶部主标纯英文**：双行纯英堆叠（如 `ZHANG ✦` / `YUANYING`），中文角色名仅在正文档案或签名处出现，绝不同行并列。
- **容器大标纯英文**：8 大容器大标 100% 纯英文大写，不加任何“装束拆解”、“配饰细节”等中文副标题。
- **纯视觉区零文字**：微距四宫格与成衣拆解内部纯靠视觉呈现，不加数字序号 `(1)-(4)` 或说明标签。
