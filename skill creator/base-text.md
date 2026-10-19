# 角色资产展示板字体规范 (base-text.md)
## Character Presentation Board Typography Specification

展示板的高奢大刊感，核心在于**全板字体的极简统一**。提示词中无需繁琐约束，只需严格定义以下三套字体：

---

### 1. 核心字体三件套 (The Typographic Triad)

1. **结构与西文标题 (Global Western & UI Headers)**
   - **字体定义**：`Razor-sharp high-contrast Didot/Bodoni editorial serif with ultra-thin hairlines (all uppercase, widely tracked)`
   - **作用范围**：顶部双行大标、右上角元数据、8 大容器标题 (`BASIC INFORMATION`, `MODEL SHEET`, `EXPRESSIONS` 等)、三视图标签 (`FRONT`, `SIDE`, `BACK`) 及工业色卡 HEX 码。容器大标与标签继承服饰主题色 `[THEME_COLOR]`。
   - **视觉效果**：类似《Vogue》大刊的高反差锐利衬线，水平发丝极细，全板统一，自带高级呼吸感。

2. **中文正文与诗意引言 (Chinese Text & Lore)**
   - **字体定义**：`Airy tracked Songti (spaced Chinese characters)`
   - **作用范围**：顶部主标题下方的设计引言、人物小传段落、核心关键词。
   - **视觉效果**：字距舒展拉开的典雅宋体，清透不凝滞。

3. **艺术签名 (Signature Script)**
   - **字体定义**：`Delicate fine-nib dip-pen cursive handwritten script in thin black ink`
   - **作用范围**：右下角专属签名 `[CharacterName]` 及下衬宣言。
   - **视觉效果**：极度优美的黑色细钢笔连笔花体手写，增添画龙点睛的个人印记。

---

### 2. 提示词标准单句注入模板 (Prompt Snippet)

在向大模型交付英文提示词时，直接注入以下简练描述即可锁定全局版式：

```text
Typography: global UI titles and container headers strictly rendered in razor-sharp high-contrast Didot editorial serif with ultra-thin hairline horizontal strokes in all uppercase, rendered in costume theme color '[THEME_COLOR]' with generous wide tracking; Chinese quotes and lore in elegant airy tracked Songti; character signature in delicate fine-nib dip-pen cursive handwritten script in thin black ink.
```

---

### 3. 四条防翻车硬规避 (Key Safeguards)

- **顶部主标纯英文与短名防挤压**：双行纯英堆叠（如 `ZHANG` / `YUANYING ✦`），中文角色名仅在正文档案或签名处出现，绝不同行并列。若英文姓氏较短（如 `LI`），引言必须严格独立换到第 3 行。
- **容器大标纯英主题色**：8 大容器大标 100% 纯英文大写 Didot 衬线体并继承主题色，不加任何“装束拆解”、“配饰细节”等中文副标题。
- **档案与关键词中英秩序**：个人档案严格保持结构化双语字段排版，严禁退化为密集英文长段；关键词必须保持 3 行中文四字词阵。
- **纯视觉区零文字零脑补**：微距四宫格与成衣拆解内部纯靠视觉呈现，不加数字序号 `(1)-(4)` 或说明标签；佩饰严格只剥离实际穿戴物，严禁脑补皮包、书籍或画册。
- **工业纯净十六进制色卡**：色卡右侧仅标显式单引号纯六位代码 `'#HEX'`，严禁添加任何 `(warm jasmine)`、`(olive)` 等括号中英文颜色名称或说明文字，杜绝扩散模型将说明文字作为画中字符打印出来。
