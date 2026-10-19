# 角色资产展示板文字排印与界面字符工程规范 (base-text.md)
## Universal Typography & On-Canvas Text Engineering Specification

> **规范地位**：本规范是 `skill creator/` 工业化工具链的**文字排版与字符工程底层宪章**。  
> **核心使命**：彻底根除现代图像扩散模型（FLUX、Midjourney、Ideogram 等）在生成角色展示板时常出现的**排印质感降级、中英字符冲突、指令污染画布（Instruction Leakage）、代码括号噪点及纯视觉区域数字污染**，建立 100% 对齐国际顶级大刊与影视设定集（以张元英黄金基准板为基准）的字形工业级工程标准。

---

## 1. 痛点溯源与排印反模式 (Typographic Anti-Patterns)

在实际展示板渲染生成中，最容易导致整张画卷从“顶级艺术大刊”跌落为“劣质淘宝详情页”的核心病灶均发生在文字排印层：

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                      展示板文字工程六大典型灾难 (Anti-Patterns)                         │
├────────────────────────────────────────────────────────────────────────────────────────┤
│ 1. 字符混排挤压 (Script Collision)  ──► 英文主标后挤入大号中文名 ('YANG ZAI ✦ 羊崽')   │
│ 2. 容器大标副标化 (Sub-Header Smog)  ──► 纯英大标下挂中文翻译 ('OUTFIT BREAKDOWN/装束拆解')│
│ 3. 过程指令泄漏 (Instruction Leak)  ──► 提示词描述词被打印到画中 ('SIGNATURE/右下角签名')  │
│ 4. 代码方括号污染 (Bracket Artifacts) ──► 关键词带程序方括号 ('[ 活力主播 ] [ 浪漫碎花 ]')    │
│ 5. 纯视觉区数字污染 (Number Badging)  ──► 微距特写画上序号角标 ('(1)', '(2)', '(3)', '(4)')   │
│ 6. 键值对机械重复 (Key-Value Stutter) ──► 字段名冗余中英堆砌 ('Traits / TRAITS:')             │
└────────────────────────────────────────────────────────────────────────────────────────┘
```

为从根本上彻底杜绝以上缺陷，所有展示板技能必须强制遵守以下底层文字公理。

---

## 2. 文字排印五大核心公理 (Core Typography Axioms)

### 2.1 字符集物理空间隔离公理 (Script Spatial Segregation Axiom)
- **铁律**：**英文主标题与中文角色名绝对禁止在同一水平行或左右紧邻混排**。
- **排布法则**：
  1. 顶部大标题（Hero Title）拥有画面的绝对视觉统领权，**必须且只能为纯英文大写两行堆叠排版**（如 `ZHANG ✦` / `YUANYING`），采用服饰主题深色高反差渲染；
  2. 中文角色名仅允许作为从属信息出现于【基本信息档案区】（如 `(张媛媛)`）以及底部的【连笔手写签名区】；
  3. 中文诗意引言以优雅拉开的字距（Tracking 1.5~2.0）居于英文主标的正下方，其下再紧随小号极细纯英大写诗意引言，形成严谨的高低音视觉天平。

### 2.2 容器大标纯英文大写 Serif 公理 (Pure English Header Axiom)
- **铁律**：**全板所有 8 大功能容器的标题必须且只能为 100% 纯英文大写 Serif，绝对禁止附带任何中文副标题**。
- **标准标题清单**：
  1. `'BASIC INFORMATION'`（个人静态档案）
  2. `'MODEL SHEET'`（居中全身定妆三视图）
  3. `'EXPRESSIONS'`（演艺多联微表情）
  4. `'OUTFIT BREAKDOWN'`（成衣立体平铺解构）
  5. `'ACCESSORIES'`（随身佩饰独立展台）
  6. `'DETAIL CLOSE-UP'`（2x2 无缝光学微距大片）
  7. `'COLOR PALETTE'`（工业 HEX 色卡系统）
  8. `'CHARACTER INTRODUCTION'`（双语角色小传）
  9. `'KEYWORDS'`（气质核心关键词）
  10. `'SIGNATURE'`（艺术连笔花体签名）
- **违规红线**：严禁在上述大标下方出现诸如“装束拆解”、“配饰细节”、“2x2 微距”、“工业色卡”、“人物小传”等任何中文翻译副标题。

### 2.3 零过程指令泄漏公理 (Zero Instruction Leakage Axiom)
- **铁律**：**提示词中的排版指令语与画面中应被渲染的字符串必须实行严格的语法物理隔离**。
- **机制**：
  - 提示词中**绝对严禁包含任何中文排版过程指示语**（如“右下角艺术签名”、“双语标签”、“居中排版”、“微距四宫格”等）；
  - 所有排版引导描述必须全部采用纯专业英文术语编写（例如 `cursive handwritten script signature`, `centered bilingual micro-label`, `seamless 2x2 macro square grid`）；
  - 唯有真正需要在画布上打印的文字，才以显式单引号 `'...'` 包裹注入。未加引号的过程性描述严禁让模型产生“这是文字内容”的歧义。

### 2.4 纯视觉陈列零文字与零编号公理 (Pristine Visual Display Axiom)
- **铁律**：**物理解构与微距特写属于纯粹的商业静物与光学大片摄影，容器内部严禁出现任何单品说明文字、引线标注或数字序号**。
- **规范细则**：
  - **OUTFIT BREAKDOWN（成衣平铺）**：纯视觉陈列，展示织物自然厚度、剪裁折痕与投影，容器内**绝无单品文字标签**；
  - **ACCESSORIES（佩饰展台）**：纯视觉独立悬浮，展示高光折射与精工质感，容器内**绝无小字注解**；
  - **DETAIL CLOSE-UP（2x2 微距）**：四幅正方形光学微距的无缝拼接，**绝对严禁出现 `(1)`, `(2)`, `(3)`, `(4)` 序号角标，绝对严禁任何文字覆层**。

### 2.5 无框悬浮字距公理 (Airy Borderless Typography Axiom)
- **铁律**：**除色卡与信息档案外，版面文字必须自然悬浮于特种艺术纸底色上，绝不使用死板的几何线框拘束**。
- **规范细则**：
  - `KEYWORDS` 容器必须采用 **3 行无边框浮动文字排版**，词与词之间通过宽敞的负空间字距（Em-space）呼吸对齐；
  - **绝对禁止出现程序员代码式的方括号 `[ ... ]`**；
  - **绝对禁止出现实体描边圆角矩形按钮框**。

---

## 3. 七阶字号与排印层级阶梯 (Typographic Hierarchy & Scale)

展示板遵循严苛的现代编辑出版学字阶比率（Modular Scale 1:1.414 或 1:1.618），构建清晰有致的 7 级阅读流：

```
+─────────────────────────────────────────────────────────────────────────────+
| Level 1: [NAME LINE 1] ✦ [NAME LINE 2]  (巨型双行大标，主色，72pt~96pt)     |
| Level 2: 中 文 诗 意 引 言 (宋体舒展 18pt) / ENGLISH QUOTE (Serif 11pt)     |
| Level 3: No. [ID] / CHARACTER PROFILE / ✦ / [OCCUPATION] (右上天平 10~14pt) |
+─────────────────────────────────────────────────────────────────────────────+
| Level 4: CONTAINER HEADERS (功能容器大标，纯英大写 Serif，14pt~16pt)        |
+─────────────────────────────────────────────────────────────────────────────+
| Level 5: BASIC INFO & INTRO (档案数据与人物小传，9pt~12pt)                  |
| Level 6: MICRO INDICATORS & HEX (三视图、表情微标、#HEX 纯色码，7pt~9pt)    |
| Level 7: SIGNATURE & MOTTO (黑色连笔手写签名与底注，24pt~36pt 手写体)       |
+─────────────────────────────────────────────────────────────────────────────+
```

### 3.1 详细层级参数对照表

| 层级 | 名称 | 语言与字型 | 排版位置 | 排印几何规范 | 严禁事项 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **L1** | 顶部主标题 | 纯英大写 Didone / Imperial Serif | 顶部左上角 | 双行垂直堆叠，服饰主题深色，尾缀优雅 `✦` | 严禁夹带中文角色名同行挤压 |
| **L2** | 诗意引言层 | 中文宋体 + 纯英大写细字 Serif | 主标题正下方 | 中文在上字距拉开，英文在下极细全大写 | 严禁使用粗黑体或无衬线随意涂抹 |
| **L3** | 右上角元数据 | 纯英大写 Tracked Serif | 顶部右上角 | `No. [ID]` 大号编号，加宽字距职业，细虚线 | 严禁插入带括号的中文翻译 |
| **L4** | 容器大标题 | 纯英大写 Serif | 8 大容器顶端 | 纯英大写，主色或沉稳黑，间距清晰 | 绝对严禁添加任何中文副标题 |
| **L5** | 档案与小传正文 | 中英双语（宋体+优雅西文） | 左栏信息区与小传区 | 档案键值清晰；小传中文在前（宋体）、英文在后 | 严禁出现 `Traits / TRAITS:` 重复键名 |
| **L6** | 微型指示标签 | 纯英 / 双语微标 | 三视图底部、微表情、色卡 | 三视图纯英 (`FRONT/SIDE/BACK`)；色卡仅纯 `#HEX`；表情居中双语小标 | 微距严禁出现数字序号 `(1)-(4)` |
| **L7** | 艺术签名与宣言 | 连笔手写体 + 纯英大写金句 | 底部右下角 | 极度优美黑色连笔手写签名 `[Name] ♡`，虚线，`- MOTTO -` | 绝对禁止出现“右下角艺术签名”文字 |

---

## 4. 题材字体家族自适应矩阵 (Typeface Genre Adaptation)

系统根据视觉反编译器提取的角色时代背景与题材气质，自适应选定最契合的西文与中文字体家族组合：

```
题材领域 ──────────► 西文字体家族 (Western Font) ──────────► 中文字体家族 (Chinese Font)
高奢时尚 / 影视名媛 ──► Didone / High-Contrast Modern Serif ──► 高级秀丽宋体 / 方正风雅宋
历史史诗 / 传统金石 ──► Trajan Imperial Roman Serif        ──► 庄严金石石刻体 / 古典康熙字典体
未来科幻 / 战术机能 ──► Technical Grotesque / DIN Monospace ──► 精密机能黑体 / 工业理性黑
潮流先锋 / 街头解构 ──► Brutalist Display Sans / Dynamic    ──► 粗砺张力黑体 / 手绘粗笔刷
```

---

## 5. 提示词工程显式单引号语法与词汇红线 (Prompt Syntax & Lexical Filter)

### 5.1 显式单引号硬锁定模板 (Explicit Quoting Specification)
所有需在最终图像中高精度完整呈现的字符，在交付提示词源码时必须使用 `'...'` 显式单引号包裹。

```text
title: stacked two-line '[NAME_LINE_1] ✦' on line 1 and '[NAME_LINE_2]' on line 2 in massive high-contrast serif rendered in deep costume theme color '[THEME_COLOR]', with strictly zero Chinese characters beside the English title, tracked Songti Chinese quote directly underneath: '[QUOTE_ZH]', followed by small tracked serif English quote: '[QUOTE_EN]'. Top-right metadata stack: 'No. [ID]' / 'CHARACTER PROFILE' / '✦' / '[OCCUPATION_CAPS]' in widely tracked uppercase serif / dotted hairline, with strictly zero parenthetical translations.

container headers: all section headers are strictly 100% pure English uppercase serif: 'BASIC INFORMATION', 'MODEL SHEET', 'EXPRESSIONS', 'OUTFIT BREAKDOWN', 'ACCESSORIES', 'DETAIL CLOSE-UP', 'COLOR PALETTE', 'CHARACTER INTRODUCTION', 'KEYWORDS', 'SIGNATURE', strictly forbidding any Chinese subtitles under container headers.

MODEL SHEET: labeled underneath in pure English serif: 'FRONT', 'SIDE', 'BACK', with zero Chinese labels.

EXPRESSIONS: each portrait labeled underneath with bilingual centered text: '[EXPR_1_ZH] / [EXPR_1_EN]', '[EXPR_2_ZH] / [EXPR_2_EN]', ...

COLOR PALETTE: vertical stack of clean rectangular color chips labeled strictly with 6-digit hex codes e.g. '#HEX_1', '#HEX_2', '#HEX_3' on the right, with zero English color name clutter.

KEYWORDS: 3 rows of borderless floating Chinese keywords with generous letter spacing, strictly zero square brackets [...], zero button boxes, and zero borders.

SIGNATURE: elegant cursive handwritten script signature of '[CharacterName] ♡' in black ink, dotted hairline, followed by centered tracked motto '- [THEMATIC_MOTTO] -', strictly zero procedural prompt leakage.
```

### 5.2 违禁词与反模式黑名单 (Lexical Blacklist)

大模型在编写 English Prompt 时，**必须通过以下违禁词自检过滤器（Filter）**：

| 违规类型 | 违禁词 / 违规写法 | 正确工程写法 | 阻断原因 |
| :--- | :--- | :--- | :--- |
| **标题混排** | `'YANG ZAI ✦ 羊崽'` | `'YANG ZAI ✦'` (两行堆叠，中文移至正文) | 破坏高奢西文版式平衡 |
| **容器副标题** | `OUTFIT BREAKDOWN / 装束拆解` | `'OUTFIT BREAKDOWN'` (纯英文大写) | 产生电商切图廉价杂音 |
| **过程词泄漏** | `SIGNATURE / 右下角艺术签名` | `SIGNATURE: elegant cursive handwritten script` | 提示词说明被直接印在画面上 |
| **程序括号** | `[ 活力主播 ] [ 浪漫碎花 ]` | `floating borderless Chinese keywords: 活力主播  浪漫碎花` | 产生程序员代码数组方框 |
| **微距角标** | `(1) eye macro (2) lip macro` | `seamless 2x2 macro square grid, strictly uncaptioned with zero numbers` | 破坏纯净光学摄影大片质感 |
| **色卡杂质** | `#C8102E Crimson Red 主装色` | `#C8102E` | 破坏专业工业色卡纯度 |
| **字段结巴** | `Traits / TRAITS:`, `Age / AGE:` | 统一层级清晰排版，无重复前缀 | 产生机械 JSON dump 乱码感 |

---

## 6. 文字排印质检雷达 (Text QA Acceptance Radar: T1~T6)

任何由母机或展示板技能生成的图片，必须对照以下 6 项文字专项雷达进行一票否决制检验：

```
                    【文字排印质检雷达 (Text QA Radar)】
                               T1: 主标纯度
                                   /\
                                  /  \
                   T6: 色卡纯净度 /    \ T2: 容器大标纯英
                                 /      \
                                /        \
                   T5: 关键词无框 \      / T3: 过程指令零泄漏
                                   \    /
                                    \  /
                                     \/
                               T4: 纯视觉无编号
```

- **[T1] 主标题纯度与双行堆叠率**：顶部大标是否为两行纯英大写 Serif 垂直堆叠？是否完全杜绝了大号中文角色名在同行左右并列挤压？
- **[T2] 容器大标纯英文率**：全板 8 大容器大标是否 100% 为纯英文大写 Serif？是否绝对杜绝了“装束拆解”、“配饰细节”、“2x2微距”、“工业色卡”、“人物小传”等中文副标题？
- **[T3] 过程指令零泄漏率**：全板文字中是否彻底根除了“右下角艺术签名”、“双语标签”等任何提示词说明性词汇？
- **[T4] 纯视觉陈列无编号率**：解构区与配饰区内部是否完全无单品小标签？2×2 微距四宫格内部是否绝对无 `(1)`, `(2)`, `(3)`, `(4)` 序号角标？
- **[T5] 关键词浮动无框率**：`KEYWORDS` 是否为 3 行无边框、无底色、无方括号 `[...]` 的透气质感字？
- **[T6] 工业色卡纯净度**：色块右侧是否仅保留纯粹的 `#` 6 位十六进制色码？是否存在多余的英文名称堆砌？

---

## 7. 静态内联交付准则 (Static Inlining Doctrine)

当母机（`Master-skill.md`）生产任何垂直领域的全新展示板技能（如游戏、影视、机甲等）时：
- 必须将本规范中规定的 **五大核心公理、单引号提示词模板与 T1~T6 质检雷达** 直接编译内联到目标单文件技能内部；
- 生产出的目标技能文件自身必须拥有自给自足的文字规范约束能力，**严禁在运行时向外引用本文件**。
