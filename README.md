<div align="center">

# 🎭 Character-Skill
### Next-Gen Industrial Character Blueprint & Presentation Board Generator
**The Production-Grade 3:4 Model Sheet Standard for AI Image Diffusion & Visual Development**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Aspect Ratio](https://img.shields.io/badge/Aspect%20Ratio-3%3A4%20Vertical-brightgreen.svg)](#layout-architecture)
[![Modality](https://img.shields.io/badge/Modality-Photo%20%7C%203D%20%7C%20Anime-orange.svg)](#orthogonal-matrix-engine)
[![Language](https://img.shields.io/badge/Language-English%20%7C%20%E4%B8%AD%E6%96%87-blueviolet.svg)](README_CN.md)

[English](README.md) · [简体中文](README_CN.md) · [Specification (ZH)](skill.md) · [Specification (EN)](Skill-En.md)

</div>

---

## 📖 Overview

**`character-skill`** is an open-source, production-grade AI Agent Skill that translates any character reference image, name, and role into a comprehensive **3:4 Vertical Character Blueprint Presentation Board** (Character Asset Sheet / VisDev Bible). 

Engineered for AAA game studios, animation houses, and concept artists, it standardizes character turnaround sheets across **FLUX, Midjourney v6, DALL-E 3, Stable Diffusion, and Gemini Imagen 3**.

### Why Character-Skill?
- 📐 **Industry-Standard 3:4 Aspect Ratio**: Abandons cramped 1:1 squares for elegant vertical artbook proportions (841×1024 / 768×1024), providing full vertical headroom and foot clearance for complete silhouettes.
- 🔄 **Omnidirectional Modality Invariance**: Strictly mirrors the input art style 1:1. Real photography stays photographic, 3D CG stays PBR-rendered, and 2D anime stays cel-shaded. Zero cross-style contamination.
- 🧩 **Orthogonal Domain Decoupling**: Separates rendering modality from industry domain. Supports **Film/Motion** (dynamic action poses, cloth physics) and **Game/Asset** (costumed quad-mesh topology, PBR material spheres).
- 🛡️ **5-Row Ergonomic Anti-Collision Grid**: An anatomical top-down layout container that completely eliminates text label overlapping and visual collision.
- 🔤 **Explicit Quoted UI Typography**: Injects legible Chinese & English bilingual pill badges, multi-angle head views, turnaround labels, and 6-expression performance strips.
- 🔒 **Two-Turn Execution Gate**: Enforces a strict two-stage workflow where prompts are previewed and confirmed before any image generation tools are triggered.

---

## 🖼️ Visual Showcase Gallery

`character-skill` adapts dynamically across all visual modalities and industry scenarios without manual tuning.

### 1. 2D Anime / Manga Illustration (`Game Asset Branch`)
> **Subject**: Linlin (林林) · Forest Spirit Mage (森林灵师)  
> **Key Features**: Tiered mint-green mesh gown, 5-row detail zoom-ins, 6 head angles, 3-view turnaround, garment silhouette breakdown, floral materials, and emotional expression strip.

<div align="center">
  <img src="assets/01_linlin_2d_anime.jpg" width="85%" alt="2D Anime Character Sheet - Linlin" />
</div>

---

### 2. Real Photography / Cinematic VisDev (`Film & Motion Branch`)
> **Subject**: Lucy Andor (露西·安多) · Modern Corporate Manager (现代职业经理人)  
> **Key Features**: Authentic 35mm optical lens rendering, visible skin pores, natural key lighting, tailored black blazer, 6 head angles, turnaround with height gauge, and dynamic motion storyboards (walking, boardroom meeting).

<div align="center">
  <img src="assets/02_lucy_andor_real_photo.jpg" width="85%" alt="Real Photography VisDev Sheet - Lucy Andor" />
</div>

---

### 3. AAA Next-Gen 3D CG (`Game Asset Branch`)
> **Subject**: Wang Yiting (王依婷) · Wudang Grandmaster (武当派掌门)  
> **Key Features**: Next-gen PBR shaders, subsurface scattering, authentic Daoist martial robes, twin sheath blades, full costumed topology quad-mesh wireframe, 8 PBR material spheres, and full-color combat expressions.

<div align="center">
  <img src="assets/03_wang_yiting_3d_game.png" width="85%" alt="Next-Gen 3D Game Asset Board - Wang Yiting" />
</div>

---

### 4. 3D Stylized Animation (`Film & Motion Branch`)
> **Subject**: Balagui (芭拉龟) · Street Dancer (街舞选手)  
> **Key Features**: High-end feature animation style (Pixar/DreamWorks aesthetic), oversized headphones, cargo joggers, 5-row street fashion callouts, turnaround, dynamic dance poses, and 6 micro-emotions.

<div align="center">
  <img src="assets/04_balagui_3d_stylized.jpg" width="85%" alt="3D Stylized Animation Sheet - Balagui" />
</div>

---

### 5. High-Aesthetic Benchmark Reference Sheet
> **Subject**: Seraphina (夕瑶) · Fantasy Visual Development  
> **Key Features**: Romantic pastel color palette, pill badges, intricate jewelry details, turnaround with reference lines, wireframe mesh, and 12 PBR material spheres.

<div align="center">
  <img src="assets/05_seraphina_benchmark.jpg" width="85%" alt="Aesthetic Benchmark - Seraphina" />
</div>

---

## 📐 Layout Architecture

The canvas strictly enforces a 3:4 vertical blueprint hierarchy, geometrically balanced to prevent overcrowding and label collisions:

```
+-----------------------------------------------------------------------------------+
| [Left 24%: Palette & Details]  | [Center 36%: Normalized Hero] | [Right 40%: Engineering & Specs] |
| - Primary title & thematic tag | - Golden-ratio center subject | - Head 6-Angle Array (2x3 grid)  |
| - 5 Physical color swatches    | - 【Pose Normalization】:      | - Key-Value Character Info Card  |
| - 7 Detail Callouts in 5 Rows: |   Relaxed Standing A-Pose     | - Full-Body 3-View Turnaround    |
|   Row 1: Face + Hair           |   revealing complete costume  | - Domain Module (Select One):    |
|   Row 2: Collar / Neckwear     | - 10% headroom, 15% footroom  |   * Film: Dynamic Motion Poses   |
|   Row 3: Torso / Sleeves       | - Soft ground contact shadow  |   * Game: Topology + PBR Spheres |
|   Row 4: Waist / Lower attire  |                               |                                  |
|   Row 5: Footwear (anchored)   |                               |                                  |
| - Single-source cursive sign   |                               |                                  |
+-----------------------------------------------------------------------------------+
| [Bottom 15%: Performance Strip] 6-expression horizontal strip (white cards + centered labels + full color) |
+-----------------------------------------------------------------------------------+
```

---

## ⚙️ Orthogonal Matrix Engine

`character-skill` synthesizes prompts along two decoupled dimensions:

```
                          ┌─► Film & Motion Branch (Default) ────► [Motion Poses + Cloth Aerodynamics]
[Input Character] ──Decouple──┤
                          └─► Game & Asset Branch (Explicit) ────► [Costumed Topology Mesh + Material Spheres]
       ▲
       │ (100% determined by reference image physical features)
       ├─► Modality A: Real Photography ──► [Optical lens fidelity, pores, studio key light; excludes 3D/Anime terms]
       ├─► Modality B: Next-Gen 3D CG   ──► [PBR shaders, subsurface scattering, ambient occlusion; excludes photo/line-art]
       └─► Modality C: 2D Anime/Manga   ──► [Crisp line-art, exquisite cel-shading; excludes 3D/photorealistic terms]
```

### Pure Positive Affirmation Rule
Modern diffusion models (FLUX, Midjourney, DALL-E 3) do not have negative prompt channels. Including words like `No 3D, without anime` triggers the **Pink Elephant Effect**, forcing the model to generate the forbidden elements. `character-skill` enforces **pure positive affirmation**, isolating vocabulary cleanly without negative phrases.

---

## 🚀 Quick Start

### 1. Integrate with AI Agents
Download `skill.md` (or `Skill-En.md`) and drop it into your agent system:
- **Antigravity / Gemini CLI**: Place in `<workspace>/skills/character-skill/SKILL.md`
- **Claude Desktop / Claude Code**: Add to your MCP custom prompts or project instructions
- **ChatGPT / Custom GPTs**: Paste the contents of `Skill-En.md` into the GPT Instructions

### 2. User Input Protocol
Provide only **three core inputs**:
```text
1. Character Reference Image (PNG/JPG)
2. Character Name: Wang Yiting (王依婷)
3. Character Role: Wudang Grandmaster (武当派掌门)
(Optional: Application scene. Defaults to Film & Motion if omitted.)
```

### 3. Two-Turn Execution Flow
```text
Turn 1: The agent checks inputs, extracts features, and outputs:
        - Track A: One-Shot Bilingual Integrated Board (Full typography)
        - Track B: Clean Plate Without Typography (For manual PS/Figma editing)
        * The agent halts and waits for your confirmation.

Turn 2: You reply "生成图片" (Generate Image) or "直接出图" (Render Now).
        * The agent invokes the image generation tool and renders your board.
```

---

## 🛠️ Prompt Injection Standard

To render pristine Chinese characters on modern diffusion models, every on-screen label is wrapped in **explicit single quotes**:

```text
- Head Portrait: 2x3 grid labeled: '正面', '3/4侧面', '侧面', '背面', '俯视', '仰视'.
- Turnaround Views: Aligned full-body turnaround labeled: '正面', '侧面', '背面'.
- Expression Strip: 6 cards labeled: '平静', '沉着', '警惕', '肃穆', '冷峻', '震慑'.
- Detail Callouts: Pill badge: 'DETAILS / 细节特写', labeled: '领口颈饰', '上装剪裁'.
```

---

## 📂 Repository Structure

```
character-skill/
├── assets/                     # High-resolution showcase artwork
│   ├── 01_linlin_2d_anime.jpg
│   ├── 02_lucy_andor_real_photo.jpg
│   ├── 03_wang_yiting_3d_game.png
│   ├── 04_balagui_3d_stylized.jpg
│   └── 05_seraphina_benchmark.jpg
├── skill.md                    # Core Skill Specification (Chinese)
├── Skill-En.md                 # Core Skill Specification (English)
├── README.md                   # English Documentation
└── README_CN.md                # Chinese Documentation
```

---

## 📄 License

Distributed under the [MIT License](LICENSE). Free for personal, commercial, and research use.
Contributions and Pull Requests are welcome!
