# Compositor

免费开源的 macOS 图像编辑器 | Free open-source macOS image editor

![Compositor 主界面 / Main Interface](docs/screenshots/main-interface.png)

---

## 项目说明 | About

**中文**：Compositor 是一款功能完整的 macOS 图像编辑器，专为图像合成与照片后期处理设计，工作流程对标 Adobe Photoshop。本仓库是 [原作者 Robbie Tilton 的 Compositor](https://github.com/robbietilton/Compositor) 的**简体中文汉化版**，采用 Photoshop 中文版专业术语进行完整本地化（883 条翻译），适合中文用户使用。

**English**: Compositor is a full-featured macOS image editor for compositing and photo work, built around a Photoshop-style workflow. This is a **Simplified Chinese (zh-Hans) localized fork** of the [original Compositor by Robbie Tilton](https://github.com/robbietilton/Compositor), with 883 professionally translated strings using standard Photoshop CN terminology.

---

## 搜索关键词 | Keywords

`Compositor 中文版` · `Compositor 汉化` · `Compositor 简体中文` · `macOS 图像编辑器` · `Photoshop 替代` · `免费修图软件 Mac` · `Compositor Chinese` · `Compositor zh-Hans` · `Compositor localized` · `macOS image editor free` · `Photoshop alternative Mac` · `open source photo editor`

---

## 安装 | Installation

**中文**：从 [GitHub Releases](https://github.com/J6meTime/Compositor/releases/latest) 下载最新版 DMG，双击挂载后拖入「应用程序」文件夹即可。

**English**: Download the latest DMG from [GitHub Releases](https://github.com/J6meTime/Compositor/releases/latest), mount it, and drag Compositor to your Applications folder.

---

## 功能特性 | Features

### 图层 | Layers
- 图层和图层组，支持不透明度和 Photoshop 全套混合模式 — Layers and folders with opacity and full Photoshop blend modes
- 图层蒙版：绘制、填充、反相、模糊、羽化 — Layer masks: paint, fill, invert, blur and feather
- 剪贴蒙版和图层组蒙版 — Clipping masks and folder masks
- 调整图层：色相/饱和度、色阶、曲线、曝光度、渐变映射、颗粒、黑白、色彩平衡、反相 — Adjustment layers: Hue/Sat, Levels, Curves, Exposure, Gradient Map, Grain, B&W, Color Balance, Invert
- 图层样式：描边、投影、颜色叠加、内阴影、外发光、内发光 — Layer effects: Stroke, Drop Shadow, Color Overlay, Inner Shadow, Outer/Inner Glow
- 向下合并 / 合并图层 / 合并图层组（⌘E） — Merge Down / Merge Layers / Merge Group (⌘E)
- 跨项目拷贝和粘贴图层 — Copy and paste layers across projects

### 变换 | Transform
- 非破坏性移动、缩放、旋转、翻转 — Non-destructive move, scale, rotate, flip
- 自由变形（⌘-拖动控制点），Shift 锁定轴向 — Free distort (⌘-drag handle), Shift locks axis
- 吸附到画布/图层边缘和中心 — Snapping to canvas/layer edges and centers
- 翻转图层和翻转画布 — Flip Layer and Flip Canvas

### 选区 | Selections
- 矩形/椭圆选框、自由/多边形套索、魔棒/对象选择 — Rectangle/Ellipse Marquee, Freehand/Polygonal Lasso, Wand/Object
- 选择主体、扩展、收缩、羽化 — Select Subject, Expand, Contract, Feather
- 内容识别填充 — Content-Aware Fill

### 绘画与修饰 | Painting & Retouching
- 画笔（大小/硬度/不透明度/平滑）、橡皮擦 — Brush (size/hardness/opacity/smoothing), Eraser
- 污点修复画笔（内容识别）— Spot Healing Brush (content-aware)
- 仿制图章（对齐/不对齐）— Clone Stamp (aligned/unaligned)
- 文字工具（T）：多行编辑、字体/大小/颜色/对齐/间距 — Type tool (T): multiline editing, font/size/color/alignment/spacing
- 渐变工具、形状工具（矩形/圆角矩形/椭圆/直线）— Gradient tool, Shape tool
- 吸管和完整拾色器 — Eyedropper and full color picker

### 调整和滤镜 | Adjustments & Filters
- Camera Raw 滤镜：光线、颜色、曲线、颜色混合器、颜色分级、细节、光学、几何 — Camera Raw filter: light, color, curves, mixer, grading, detail, optics, geometry
- 高斯模糊、动感模糊、添加杂色、晕影、绽放发光 — Gaussian/Motion Blur, Add Noise, Vignette, Bloom/Glow
- 色调对比、镜头校正、移除背景 — Tonal Contrast, Lens Correction, Remove Background
- 实时预览，上次滤镜（⌃⌘F）— Live previews, Last Filter (⌃⌘F)

### 画布和文件 | Canvas & Files
- 标签页管理多个项目 — Multiple projects in tabs
- 搜索命令（⌘F）、切换全屏（F）— Search Commands (⌘F), Toggle Fullscreen (F)
- 标尺（⌘R）、参考线、布局网格、吸附 — Rulers (⌘R), guides, layout grid, snapping
- 裁剪（支持比例 3:4、9:16）— Crop with ratios (3:4, 9:16)
- 导入：JPEG、PNG、HEIC、TIFF、SVG、相机 RAW、PSD/PSB — Import: JPEG, PNG, HEIC, TIFF, SVG, camera RAW, PSD/PSB
- 导出 JPEG 实时预览（⇧⌥⌘S）— Export JPEG with live preview (⇧⌥⌘S)
- Photoshop 风格键盘快捷键，可自定义 — Photoshop-style shortcuts, remappable
- 通过 Sparkle 自动更新 — Automatic updates via Sparkle

### 支持 AI 代理 | Works with AI Agents
- `.comp` 项目 = PNG 图层文件夹 + 清单文件；打开的项目在外部修改时实时更新 — `.comp` projects are folders of PNG layers + manifest; open projects update live when written externally
- 详见 [编写 Compositor 项目](docs/writing-comp-files.md) — See [Writing Compositor projects](docs/writing-comp-files.md)

---

## 系统要求 | Requirements

- macOS 26.0 或更高版本，Apple 芯片 — macOS 26.0+ on Apple silicon
- Xcode 26+（从源码构建）— Xcode 26+ (to build from source)

## 构建 | Building

打开 `Compositor.xcodeproj`，运行 **Compositor** scheme — Open `Compositor.xcodeproj` and run the **Compositor** scheme.

---

## 版权与致谢 | Credits & License

**原作者 | Original Author**: [Robbie Tilton](https://github.com/robbietilton) — [原项目仓库 | Original Repository](https://github.com/robbietilton/Compositor) — [官网 | Website](https://robbietilton.com/compositor)

**汉化 | Chinese Localization**: 本仓库在原项目基础上新增完整的简体中文（zh-Hans）本地化，采用 Photoshop 中文版专业术语。This fork adds full Simplified Chinese (zh-Hans) localization with professional Photoshop CN terminology.

**许可 | License**: MIT — 详见 [LICENSE](LICENSE) — See [LICENSE](LICENSE).

> 本项目基于 Robbie Tilton 的开源项目 Compositor（MIT 许可）进行汉化，遵循同一 MIT 许可协议。This project is a localized fork of Robbie Tilton's open-source Compositor (MIT License), distributed under the same MIT License.
