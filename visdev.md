---
name: visdev-costume-bible
description: "国际顶级全模态角色视觉解构与设定集生成元引擎（Visual Decompilation & Costume Bible Meta-Engine）。面向任意题材角色（3D皮克斯动画/日本动漫二次元/影视写实摄影/次世代游戏CG/男女老少机甲），严格遵循 Rule.md 2:3 纵向无黑线骨架，实现模态物理原生守恒与参考图真身零脑补解构：主题色双行大标、居中九头身定妆三视图、戏剧张力微表情肖像、高定静物立体平铺解构(Flat-lay)、配饰悬浮展台、2x2模态特征微距四宫格、工业HEX色卡及双语小传手写签名。"
---

# Visual Decompilation & Costume Bible Meta-Engine (visdev.md)
## 国际顶级全模态角色视觉解构 · 剧组服化道定妆圣经生成元引擎

> **最高宪法**：本 Skill 全面继承并在底层严格受制于 [Rule.md](Rule.md)。
> **核心法则**：**“骨架是绝对刚性的工业规范，内容是 100% 忠实于参考图的无限自适应”**。彻底杜绝打补丁思维，彻底杜绝角色硬编码！

---

## 1. 核心执行门禁 (Execution Gate)

- **信息完整门禁**：在未集齐【角色参考图】、【角色名称】、【角色职业/设定】这 3 项核心要素之前，仅进行针对性提问补齐，绝不提前输出提示词方案。
- **时间轴与出图门禁**：第一轮身份为【纯文本视觉解构总监】，交付完整提示词源码后必须原地待命等待。用户的初始需求（如“帮我做一张展示板”）属于业务意图，绝对严禁作为出图授权；唯有在提示词交付完成之后、用户在【后续独立新消息】中明确回复“生成图片”或“直接出图”，第二轮方可启动生图工具。

---

## 2. 系统架构与三大系统级元法则 (The Three Meta-Laws)

系统不当臆想捏造的编剧，而是一台**高精度的“视觉解构与设定集排印仪”**：

```
                    【用户上传任意题材角色参考图 (3D皮克斯 / 日本动漫 / 写实摄影 / 游戏CG)】
                                                     │
                                                     ▼
                        ┌────────────────────────────────────────────────────────┐
                        │              视觉反编译器 (Visual Decompiler)          │
                        │    客观提取：艺术风格模态、服装拓扑、配饰道具、面料质感 │
                        └────────────────────────────────────────────────────────┘
                                                     │
        ┌─────────────────────────┬──────────────────────────┬─────────────────────────┐
        ▼                         ▼                          ▼                         ▼
【元法则 1: 模态物理原生守恒】  【元法则 2: 真身零脑补解构】  【元法则 3: 刚性容器装配】  【通道: 镜头表演微表情】
· 3D皮克斯 ──► 顶级黏土微光   · 衣服穿什么就平铺什么      · 严格 2:3 纵向艺术纸画幅   · 斯坦尼斯拉夫斯基6维弧线
· 日本动漫 ──► 赛璐珞精美线稿 · 佩戴什么就悬浮什么        · 纯白留白，零黑实线切割    · 微表情配合手部肢体微动
· 影视写实 ──► 35mm哈苏质感   · 2x2微距自适应题材焦点     · 扁平8大容器，无中层大标   · 严格杜绝呆滞大头照
· 次世代CG ──► UE5 PBR渲染    · 色卡从像素吸取真HEX码     · 纯视觉零文字，色卡纯HEX   · 角色动态编号与专属职业
```

### 元法则 1：模态物理原生守恒 (Native Modality Invariance)
系统内置四大原生渲染模态，依据参考图物理特征 **100% 自动锁定，全板同频**，绝不跨风格强行转换：
1. **【Modality 3D-Stylized】皮克斯/动画风格**：
   - 整板（三视图、微表情、平铺衣服、微距特写）原生呈现皮克斯/梦工厂特有的圆润体态、次表面散射微光（SSS）、柔和黏土与精细绒布质感、大眼瞳孔光斑与生动夸张表情。**绝不强加真人粗糙毛孔！**
2. **【Modality 2D-Anime】日本动漫/手绘插画**：
   - 整板原生呈现京都动画/新海诚剧场版动画像素级精致线稿、细腻赛璐珞平涂、高光通透的漫画大眼、平面插画风服装平铺与二次元画风排版。**绝不强行转成 3D 泥人！**
3. **【Modality Realistic】真实摄影/电影定妆**：
   - 整板原生呈现 35mm 光学镜头真实焦段、微孔自然人像肤质、真实光线反弹、高奢商业成衣静物摄影质感。
4. **【Modality Game-CG】次世代 3D 游戏 CG**：
   - 整板原生呈现虚幻引擎 5（Unreal Engine 5）级 PBR 材质解算、高多边形拓扑感、微型机械咬合与发光材质能量流动。

### 元法则 2：“真身解构”零脑补提取机制 (Zero-Hallucination Extraction)
提示词构建时，强制要求大模型**完全基于用户参考图的真实像素进行客观转译**：
- **衣服绝不瞎编**：参考图身上穿什么，平铺区就精准拆解平铺那 3~5 件外装单品！
  - 若是皮克斯街舞少年，平铺区就拆解**拼色连帽卫衣、多袋束脚工装裤与复古滑板鞋**；
  - 若是日漫水手服少女，平铺区就拆解**深蓝水手领上衣、百褶短裙、中筒袜与黑色乐福鞋**；
  - 若是科幻机甲战士，平铺区就拆解**轻型外挂复合胸甲、柔性动力内衬衣、战术护膝重装长裤与合金快拆战靴**；
  - 若是古代剑客，平铺区就拆解**宽袖交领外袍、护心甲革带、暗纹练功长裤与云头皂靴**。
- **配饰绝不瞎猜**：参考图佩戴什么就独立悬浮什么！
  - 戴着头戴式耳机就展示耳机，戴着发夹就展示发夹，挂着佩剑就展示佩剑，空手就展示随身信物，**绝不凭空塞进不搭界的红宝石耳坠或珍珠项链**！
- **2×2 微距焦点绝不写死口红眼线**：根据题材自适应匹配最具辨识度的 4 个微距焦点：
  - **动漫角色**：聚焦于 1. 漫画眼瞳星光高光 2. 嘴角微笑弧度 3. 灵动手绘发丝线稿 4. 服装特征印花/徽章；
  - **皮克斯角色**：聚焦于 1. 灵动大眼玻璃球反射 2. 黏土面颊柔和微光 3. 毛线帽/毛发细柔绒毛 4. 连帽卫衣金属抽绳/拉链扣；
  - **写实角色**：聚焦于 1. 人类真实虹膜与睫毛 2. 唇纹或下颌轮廓 3. 发丝高光流向 4. 蕾丝刺绣/皮革荔枝纹/碳纤维纹理；
  - **机甲角色**：聚焦于 1. 战术目镜 HUD 光圈 2. 呼吸面罩过滤阀 3. 碳纤装甲边缘拉丝 4. 动力关节咬合齿轮。
- **色卡绝不瞎起名**：
  - 从参考图身上吸取真实存在的 5~6 种主色，**直接输出纯十六进制 HEX 码**（如 `#2B2D42`, `#E63946`），零多余英文色彩名称堆砌。
- **元数据绝不硬塞固定职业与编号**：
  - 右上角职业标签直接提取参考图的角色本质（如 `STREET DANCER`, `FOREST MAGE`, `SPACE PILOT`, `DETECTIVE`, `CYBER VANGUARD` 等），编号根据任务动态派发（如 `ARCHIVE No. 01`）。

### 元法则 3：结构容器刚性，内容无限自由 (Rigid Containers, Infinite Freedom)
无论面对什么画风、什么角色，以下结构契约 100% 保持刚性：
1. **严格 2:3 纵向黄金画幅（800×1200 / 1024×1536）**，释放 12.5% 纵向留白，全身立姿不切脚；
2. **纯白（Pure Clean White）或微暖特种艺术纸底色，严格无任何横贯屏幕的粗黑实线与表格边框**；
3. **顶部主题色巨型双行大标 + 右上角垂直元数据平衡天平**；
4. **居中九头身定妆三视图（FRONT / SIDE / BACK）舒展站立 A-pose**；
5. **扁平化 8 大原子容器**，绝不人为添加 `DECONSTRUCTION` 或 `THE THREE-VIEW` 等中层大标题；
6. **纯视觉陈列容器洁净律**：成衣平铺与佩饰展台零单品文字标注，微距四宫格零 1, 2, 3, 4 序号与文字说明；
7. **色卡纯 `#HEX` 码**，无多余英文描述。

---

## 3. 2:3 扁平化八大原子功能容器几何排布 (Layout Architecture)

```
+---------------------------------------------------------------------------------------------------+
| [顶部大标题与引言 12%] (纯白无框背景，双重天平构图)                                               |
|  巨型双行高反差大标（提取服饰主色）：[NAME LINE 1] ✦                   ARCHIVE No. XX             |
|                                    [NAME LINE 2]                     CHARACTER PROFILE          |
|                                                                      ✦                          |
|  双语精致引言：[中 文 诗 意 设 计 引 言 ， 适 度 拉 开 字 距 。]       [DYNAMIC ROLE IN CAPS]     |
|  [ENGLISH THEMATIC POETIC QUOTE IN ELEGANT SERIF CAPITALS.]          ·························· |
+---------------------------------------------------------------------------------------------------+
| [上半部 50%: 角色演艺现场] (空间自然留白分隔，严格无黑线)                                         |
| [容器 1: 个人静态档案]        | [容器 2: 全身定妆三视图]             | [容器 3: 演艺肖像 2x3]     |
| BASIC INFORMATION             | MODEL SHEET                          | EXPRESSIONS               |
|                               |                                      |                           |
| 角色名 (小字)                 | 舒展直立站姿 (九头身比例):           | 白底轻柔卡片，生动手势:   |
| [Name En] ([Name Zh])         | [正面直立]   [侧面90度]   [背面直立] | [肖像 1]     [肖像 2]     |
|                               | FRONT          SIDE          BACK    | 表情双语标签 表情双语标签 |
| 职业: [Role Zh] / [Role En]   |                                      |                           |
| 年龄 / AGE: [Age]             | · 展现服装真实版型与模态物理光影     | [肖像 3]     [肖像 4]     |
| 身高 / HEIGHT: [Height]       | · 专业柔光棚拍/光影渲染，真实接触投影| 表情双语标签 表情双语标签 |
| 外观特征:                     | · 顶部与脚部拥有 12%~15% 呼吸留白    |                           |
| · 发型/发色: [Hair Details]   |                                      | [肖像 5]     [肖像 6]     |
| · 标志特征: [Distinct Traits] |                                      | 表情双语标签 表情双语标签 |
| 气质标签: [Keywords 1-6]      |                                      | (配合微动眼神与手部动作)  |
+---------------------------------------------------------------------------------------------------+
| [下半部 第一层 24%: 四大实体物理解构列] (严格并排，中间绝无横切死黑线)                            |
|                                                                                                   |
| [容器 4: 成衣立体平铺] | [容器 5: 佩饰独立悬浮] | [容器 6: 2x2 微距四宫格] | [容器 7: 工业色卡系统]|
| OUTFIT BREAKDOWN      | ACCESSORIES            | DETAIL CLOSE-UP          | COLOR PALETTE         |
| 商业静物立体展陈:     | 标志性道具悬浮展台:    | 2x2 无缝高精微距大片:    | 纯净矩形色块垂直堆叠: |
| 客观拆解参考图3~5件   | 客观提取参考图2~4件    | 1. [焦点1: 眼部/光圈]    | #HEX_1 (主装色)       |
| 真实外装(外衣/内搭/下 | 随身核心信物(耳机/配饰 | 2. [焦点2: 面容/局部]    | #HEX_2 (辅装色)       |
| 装/鞋履/护具)，带真实 | /挂件/法器)，通透质感。| 3. [焦点3: 发丝/头饰]    | #HEX_3 (配饰色)       |
| 模态厚度与阴影。      |                        | 4. [焦点4: 核心材质/纹理]| #HEX_4 (细节色)       |
| 【绝无文字标注！】    | 【绝无文字标注！】     | 【绝无数字！绝无文字！】 | #HEX_5 (点缀色)       |
|                       |                        |                          | (右侧仅标纯HEX码！)   |
+---------------------------------------------------------------------------------------------------+
| [下半部 第二层 14%: 灵魂注脚与艺术签名] (容器 8: LORE & IDENTITY)                                 |
|                                                                                                   |
| [左栏 42%: 双语人物小传]      | [中栏 28%: 核心标签线框组]          | [右栏 30%: 艺术连笔花体签名]|
| CHARACTER INTRODUCTION        | KEYWORDS                            | SIGNATURE                   |
|                               |                                     |                             |
| 典雅中文诗意小传段落(3~4行)   | 2行x3列独立圆角白底线框矩形标签：   | 极度优美的黑色连笔艺术手写名|
| 下方紧跟极细英文小字段落(3~4行| [ 核心词 1 ] [ 核心词 2 ] [ 词 3 ]  | [Character Name] ♡          |
| 深入刻画镜头前的内心戏剧力量  | [ 核心词 4 ] [ 核心词 5 ] [ 词 6 ]  | ··························  |
|                               |                                     | - [专属设计宣言金句] -      |
+---------------------------------------------------------------------------------------------------+
```

---

## 4. 提示词生成语法与四大模态动态注入规范 (Prompt Syntax)

### 4.1 四大原生模态画风基调代码库 (依据参考图动态选用)

构建提示词前缀时，大模型必须根据参考图的风格，从以下四大模态基调中**精准选用对应的渲染基调，严禁张冠李戴**：

- **【选用 A：3D-Stylized 皮克斯/动画模态】**：
  ```text
  Top-tier 3D stylized animation visual development presentation board, Pixar and DreamWorks character artbook aesthetic. Strictly borderless clean pure white fine-art paper backdrop, NO horizontal solid black dividing rules, NO tabular frames, elegant negative space and breathing room. Soft volumetric studio lighting, rich stylized subsurface scattering skin, smooth stylized fabric and clay shaders, expressive animated poses, crisp 3D asset render, 8k resolution, masterpiece.
  ```

- **【选用 B：2D-Anime 日本动漫/二次元模态】**：
  ```text
  Masterpiece 2D Japanese anime visual development character sheet, high-end animation artbook editorial layout, Kyoto Animation and Makoto Shinkai visual aesthetics. Strictly borderless clean pure white paper backdrop, NO horizontal solid black dividing rules, NO tabular frames, elegant breathing negative space. Crisp elegant hand-drawn line-art, vibrant delicate cel-shading, luminous expressive anime eyes, beautifully illustrated fashion flat-lay, immaculate publication print quality, 8k resolution.
  ```

- **【选用 C：Realistic 真实摄影/电影定妆模态】**：
  ```text
  High-end cinematic visual development costume design bible, luxury editorial fashion presentation board. Strictly borderless clean pure white fine-art paper backdrop, NO horizontal solid black dividing rules, NO tabular frames, elegant negative space and natural breathing room. Studio key spotlight lighting, natural dewy skin texture, subtle rim lighting pop-out effect, 35mm optical lens clarity, authentic material physics, commercial still-life product photography, 8k resolution, masterpiece.
  ```

- **【选用 D：Game-CG 次世代游戏角色模态】**：
  ```text
  AAA next-gen video game character visual development concept artbook sheet, Unreal Engine 5 high-fidelity render aesthetic. Strictly borderless clean pure white studio background, NO horizontal solid black dividing rules, NO tabular frames, sophisticated negative space. Studio key lighting, advanced PBR micro-surface materials, quad-mesh topology precision, dynamic specular highlights, crisp asset presentation, 8k resolution, masterpiece.
  ```

### 4.2 汉字、色码与界面单引号注入模板 (Zero-Hardcoding Injection)
在生成的 English Prompt 中，所有界面需呈现的字样必须使用 `'...'` 显式包裹，且所有变量全部动态绑定：
- **顶部双行标题与引言**：
  `title: stacked two-line '[NAME_LINE_1] ✦' on line 1 and '[NAME_LINE_2]' on line 2 in massive high-contrast typeface rendered in deep costume theme color '[THEME_COLOR]', top-right metadata stack: 'ARCHIVE No. [DYNAMIC_ID]' / 'CHARACTER PROFILE' / '✦' / '[DYNAMIC_OCCUPATION_CAPS]' / dotted hairline, bilingual quote: '[QUOTE_ZH] [QUOTE_EN]'`
- **三视图标签**：`labeled underneath: 'FRONT', 'SIDE', 'BACK'`
- **表演微表情**：
  `labeled underneath: '[表情1_ZH] / [EXPR_1_EN]', '[表情2_ZH] / [EXPR_2_EN]', '[表情3_ZH] / [EXPR_3_EN]', '[表情4_ZH] / [EXPR_4_EN]', '[表情5_ZH] / [EXPR_5_EN]', '[表情6_ZH] / [EXPR_6_EN]'`
- **模块纯净大标（严禁中层分类大标）**：
  `'BASIC INFORMATION'`, `'MODEL SHEET'`, `'EXPRESSIONS'`, `'OUTFIT BREAKDOWN'`, `'ACCESSORIES'`, `'DETAIL CLOSE-UP'`, `'COLOR PALETTE'`, `'CHARACTER INTRODUCTION'`, `'KEYWORDS'`, `'SIGNATURE'`
- **工业色卡系统**：
  `COLOR PALETTE: vertical stack of clean rectangular color chips sampled directly from the character image, labeled strictly with 6-digit hex codes e.g. '#HEX_1', '#HEX_2', '#HEX_3', '#HEX_4', '#HEX_5' on the right, with zero English color name clutter`
- **纯视觉陈列铁律**：
  `OUTFIT BREAKDOWN and ACCESSORIES must be pure commercial still-life product displays featuring the character's actual decomposed garments and equipment with realistic material thickness and subtle drop shadows, with ZERO text labels underneath the items. DETAIL CLOSE-UP must be a seamless 2x2 macro square grid with ZERO numbers and ZERO captions.`

### 4.3 静默纯正向词法 (Pure Positive Affirmation)
严禁在提示词中使用任何 "No 3D, without anime" 等否定词汇，严禁生成 Negative Prompt 代码块。全篇仅使用纯正向的美术设计、模态渲染与画册排印专业词汇！

---

## 5. 两轮标准化交互工作流 (Two-Turn Sequential Workflow)

```
+-----------------------------------------------------------------------------------+
| 【Turn 1: 输入校验、真身反编译与提示词源码交付】                                  |
|  1. 门禁检查三项输入：[角色参考图]、[角色名称]、[角色职业/设定]                           |
|     - 缺任意一项：立即礼貌询问补齐，严禁自动编造假名                                     |
|  2. 视觉反编译：客观提取参考图模态、真身成衣清单、真实佩饰、2x2微距焦点、HEX码与双语小传   |
|  3. 源码交付：在独立 Markdown 代码块中输出完整双语提示词源码（方案A整板 + 方案B纯净底板）  |
|  4. 阶段停机：输出确认引导，本轮交付完毕后原地等待，绝不调用任何生图工具                 |
+-----------------------------------------------------------------------------------+
                                         │
                        用户发送独立新消息：“生成图片” / “直接出图”
                                         ▼
+-----------------------------------------------------------------------------------+
| 【Turn 2: 授权执行出图与全向工业级验收】                                          |
|  1. 启动生图工具，携带参考图路径与优化提示词发起高精渲染                                 |
|  2. 交付图片，并对照 Rule.md 工业验收雷达输出专业验收报告                                |
+-----------------------------------------------------------------------------------+
```

#### 5.1 Turn 1 执行细则
- **三要素门禁询问模板**（缺失输入时调用）：
  > “为了为你设计符合国际顶级标准的 2:3 角色视觉解构与定妆概念档案（VisDev & Costume Bible），请补充提供：
  > 1. 角色参考图（用于客观提取画风模态、妆造发型与真实服装物理细节）
  > 2. 角色名称（用于全板双行主题色大标与手写花体签名）
  > 3. 角色职业 / 剧目设定（用于推导角色小传、气质评级与设计理念）
  > （注：生日、身高、真实 HEX 色值、服装平铺拆解物料、佩饰与双语小传，系统将通过视觉反编译引擎全自动智能提取，无需繁琐输入）”
- **源码输出格式**：
  必须在独立代码块中完整输出：
  * `方案 A：一键整板中英双语角色定妆概念档案生成（ENGLISH PROMPT & 中文对照）`
  * `方案 B：纯净无字底板生成（ENGLISH PROMPT - CLEAN PLATE 供后期在 PS/InDesign 精确填字）`
- **【确认引导】**：
  代码块输出完毕后，**必须输出以下确认引导并结束第一轮交互，等待用户确认指示，此轮不调用生图工具**：
  > “以上是基于你的角色参考图完成‘真身零脑补解构’的 2:3 角色视觉开发与服化道定妆圣经（VisDev & Costume Bible）完整提示词。
  > 严格遵循 Rule.md 刚性架构：主题色双行大标、九头身全身三视图、高定立体平铺解构、2x2四宫格微距与工业HEX色卡，纯白无黑线留白排版。
  > 请确认提示词细节。确认无误后请回复**‘生成图片’**或**‘直接出图’**，我将在下一轮为你调用工具生成；如需微调也可以直接提出。”

#### 5.2 Turn 2 执行细则
- 只有收到用户包含“生成图片”或“直接出图”的消息后，方可启动工具出图。
- 出图完成后，执行全向工业验收（对照 `Rule.md` 8 项雷达）。
