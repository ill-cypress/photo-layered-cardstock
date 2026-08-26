# Photo Layered Cardstock

[English](#english) · [中文](#中文)

## English

`photo-layered-cardstock` is a Codex skill that transforms a source photograph into a clean, unframed cardstock diorama. It reconstructs the photographed scene as multiple separate paper sheets stacked in physical depth and renders the result from a slight oblique angle so the sheet thickness, exposed edges, spacing, and cast shadows remain visible.

### Core principle

> One spatial depth plane = one separate physical cardstock sheet.

Elements may share a sheet only when they occupy the same depth plane in the source photograph. Foreground, main subject, midground, background, and sky content must not be flattened onto a single sheet.

### What the skill preserves

- The recognizable subject and overall scene
- Major silhouettes, placement, scale relationships, and overlaps
- The source composition and aspect ratio unless another format is requested
- Source-derived colors, simplified into broad matte paper shapes

### What the skill emphasizes

- Multiple thick cardstock sheets stacked from front to back
- A slight oblique view instead of a flat front-facing view
- Visible paper edges, air gaps, contact shadows, and soft cast shadows
- Clean, elegant paper-cut forms with restrained detail
- Strong physical depth rather than surface decoration

### Hard constraints

- No box, outer frame, border, mat, bezel, rim, backing board, stand, or enclosing walls
- No flat poster-like papercut illustration
- No single-layer or mixed-depth sheet composition
- No overly intricate micro-detail
- No invented or arbitrarily rearranged primary subjects
- No text, caption, label, or watermark in the generated artwork

### Installation

Ask Codex to install this repository with the built-in skill installer:

```text
Use $skill-installer to install https://github.com/ill-cypress/photo-layered-cardstock
```

Codex detects newly installed skills automatically. If the skill does not appear, restart Codex.

### Usage

Attach a source photograph and invoke the skill explicitly:

```text
Use $photo-layered-cardstock to transform this photo into an unframed layered-cardstock diorama.
```

The skill may also activate automatically when a request clearly asks for this specific photo-to-cardstock transformation.

### Workflow

1. Identify the main subject and meaningful depth planes.
2. Group visual elements strictly by spatial depth.
3. Convert every depth plane into a separate cardstock sheet.
4. Stack the sheets in physically correct front-to-back order.
5. Render the construction from a slight oblique angle.
6. Use coherent lighting and shadows to make the separation unmistakable.

### Repository structure

```text
photo-layered-cardstock/
├── SKILL.md                  Core behavior and constraints
├── agents/openai.yaml        Codex UI metadata and default prompt
└── references/visual-spec.md Detailed prompt and visual QA guidance
```

This skill creates a rendered image, not a fabrication-ready cutting template.

---

## 中文

`photo-layered-cardstock` 是一个 Codex skill，用于把输入照片转换成干净、无外框的分层卡纸立体景。它会按照照片中的空间深度重建场景，将不同深度分别放在多张独立卡纸上，再从轻微斜侧角度呈现，使纸张厚度、裸露纸边、层间距离和投影清晰可见。

### 核心原则

> 一个空间深度层 = 一张独立的实体卡纸。

只有处于同一空间深度的元素才能共用一张卡纸。前景、主体、中景、背景和天空不能被压平到同一张纸上。

### Skill 会保留什么

- 可识别的主体和完整场景
- 主要轮廓、位置、比例关系和遮挡关系
- 原照片构图和宽高比，除非用户另有要求
- 从原照片提取并简化成大块哑光纸色的配色

### Skill 会重点强化什么

- 多张厚卡纸从前到后依次叠放
- 轻微斜侧视角，而不是平直正面视角
- 清晰可见的纸边、空气间隙、接触阴影和柔和投影
- 干净、优雅、细节克制的剪纸造型
- 真实物理纵深，而不是表面装饰

### 强制约束

- 不得出现盒体、外框、边框、卡纸衬框、边缘外壳、背板、底座或包围墙
- 不得生成平面海报式剪纸插画
- 不得生成单层结构，也不得在同一张纸上混合多个深度层
- 不得使用过度复杂的微小细节
- 不得虚构、随意删除或重新排列主要主体
- 生成画面中不得出现文字、说明、标签或水印

### 安装

让 Codex 使用内置的 skill installer 安装这个仓库：

```text
Use $skill-installer to install https://github.com/ill-cypress/photo-layered-cardstock
```

Codex 通常会自动检测新安装的 skill。如果没有显示，请重启 Codex。

### 使用方法

上传一张源照片，然后显式调用：

```text
Use $photo-layered-cardstock to transform this photo into an unframed layered-cardstock diorama.
```

当请求明确描述了这种“照片转分层卡纸立体景”的需求时，Codex 也可能自动启用该 skill。

### 工作流程

1. 识别主体和有意义的空间深度层。
2. 严格按照空间深度对画面元素分组。
3. 将每个深度层转换成一张独立卡纸。
4. 按照正确的物理顺序从前到后叠放卡纸。
5. 从轻微斜侧角度呈现整个结构。
6. 使用一致的光照和阴影清楚表现层间分离。

### 仓库结构

```text
photo-layered-cardstock/
├── SKILL.md                  核心行为与约束
├── agents/openai.yaml        Codex 界面元数据与默认提示
└── references/visual-spec.md 详细生成提示与视觉质量检查规范
```

这个 skill 用于生成渲染图像，不用于制作可直接生产的切割模板。
