# Compositor

> **中文介绍见下方** / [English](#english) · [中文](#中文)

---

<a id="english"></a>

## English

Compositor is a full-featured, free and open-source macOS image editor for compositing and photo work, built around a Photoshop-style workflow.

Adobe Photoshop costs too much, and tools like GIMP don't feel familiar enough to stay in flow. Compositor fills that gap — with all the tools needed to create a pixel-perfect final image, completely free and open source.

This is a **Chinese-localized fork** of the original [Compositor by Robbie Tilton](https://github.com/robbietilton/Compositor), with full Simplified Chinese (zh-Hans) localization using professional Photoshop CN terminology.

![Compositor Main Interface](docs/screenshots/main-interface.png)

### Installation

Download the latest release from [GitHub Releases](https://github.com/J6meTime/Compositor/releases/latest).

### Features

**Layers**
- Layers and folders, with opacity and Photoshop's full set of blend modes
- Layer masks: paint, fill, invert, blur and feather; link or unlink to transform independently
- Clipping masks and folder masks
- Adjustment layers: Hue/Saturation, Levels, Curves, Exposure, Gradient Map, Grain, Black & White, Color Balance, Invert, Gaussian Blur, Motion Blur, Noise
- Layer effects: Stroke, Drop Shadow, Color Overlay, Inner Shadow, Outer/Inner Glow (GPU-rendered, editable anytime)
- Merge Down / Merge Layers / Merge Group (⌘E)
- Duplicate, rename inline, reorder, nest by drag and drop; Option-drag to duplicate
- Copy and paste whole layers and folders across projects

**Transform**
- Non-destructive move, scale, rotate, flip — full resolution preserved
- Free distort (⌘-drag a handle), Shift to lock axis
- Transform multiple layers or folders together
- Snapping to canvas/layer edges and centers with guides
- Flip Layer and Flip Canvas, horizontal and vertical

**Selections**
- Rectangle/Ellipse Marquee, Freehand/Polygonal Lasso, Magic Wand (color) and Object (trace)
- Select Subject, Expand, Contract, Feather
- Add/subtract selections, move outline or pixels
- Content-Aware Fill

**Painting & Retouching**
- Brush with size, hardness, opacity, smoothing (B/E), Shift for straight lines
- Spot Healing Brush (content-aware)
- Clone Stamp (aligned/unaligned, single/all layers)
- Blur tool, Gradient tool, Shape tool (rectangles, rounded rectangles, ellipses, lines)
- Type tool (T): inline multiline editing, font/size/color/alignment/spacing
- Eyedropper and full color picker

**Adjustments & Filters**
- Camera Raw filter: light, color, curves, color mixer, color grading, detail, optics, geometry
- Levels (with Auto), Curves, Hue/Saturation, Exposure, Gradient Map, Grain, Black & White, Color Balance, Invert
- Gaussian/Motion Blur, Add Noise, Vignette, Bloom/Glow, Tonal Contrast, Lens Correction, Remove Background
- Live previews, Last Filter (⌃⌘F)

**Canvas & Files**
- Multiple projects in tabs
- Search Commands (⌘F), Toggle Fullscreen (F)
- Rulers (⌘R), guides, layout grid, Snap To
- Crop with snapping and ratios (3:4, 9:16)
- Canvas Size, Image Size, Trim
- Import: JPEG, PNG, HEIC, TIFF, SVG, camera RAW, Photoshop PSD/PSB (8-bit RGB)
- Export JPEG with live preview (⇧⌥⌘S), Copy Merged
- Photoshop-style keyboard shortcuts, remappable
- Automatic updates via Sparkle

**Works with AI agents**
- `.comp` projects are folders of PNG layers + manifest; open projects update live when written externally. See [Writing Compositor projects](docs/writing-comp-files.md)

### Requirements
- macOS 26.0 or later on Apple silicon
- Xcode 26+ (to build from source)

### Building
Open `Compositor.xcodeproj` and run the **Compositor** scheme.

### Credits

- **Original project**: [Compositor](https://github.com/robbietilton/Compositor) by [Robbie Tilton](https://github.com/robbietilton)
- **Chinese localization**: This fork adds full Simplified Chinese (zh-Hans) localization with professional Photoshop CN terminology

### License

MIT — see [LICENSE](LICENSE).

---

<a id="中文"></a>

## 中文

Compositor 是一款功能完整、免费开源的 macOS 图像编辑器，专为图像合成与照片后期处理设计，工作流程对标 Photoshop。

Adobe Photoshop 太贵，GIMP 等工具又不够顺手。Compositor 填补了这个空白——提供创建完美图像所需的全部工具，完全免费开源。

本项目是 [Robbie Tilton 的原版 Compositor](https://github.com/robbietilton/Compositor) 的**简体中文汉化分支**，采用 Photoshop 中文版专业术语进行完整本地化（883 条翻译）。

![Compositor 主界面](docs/screenshots/main-interface.png)

### 安装

从 [GitHub Releases](https://github.com/J6meTime/Compositor/releases/latest) 下载最新版本。

### 功能特性

**图层**
- 图层和图层组，支持不透明度和 Photoshop 全套混合模式
- 图层蒙版：绘制、填充、反相、模糊、羽化；可取消关联以独立变换
- 剪贴蒙版和图层组蒙版
- 调整图层：色相/饱和度、色阶、曲线、曝光度、渐变映射、颗粒、黑白、色彩平衡、反相、高斯模糊、动感模糊、杂色
- 图层样式：描边、投影、颜色叠加、内阴影、外发光、内发光（GPU 渲染，随时编辑）
- 向下合并 / 合并图层 / 合并图层组（⌘E）
- 复制、内联重命名、拖拽排序和嵌套；Option-拖动复制
- 跨项目拷贝和粘贴整个图层或图层组

**变换**
- 非破坏性移动、缩放、旋转、翻转——始终保留原始分辨率
- 自由变形（⌘-拖动控制点），Shift 锁定轴向
- 多图层或图层组一起变换
- 吸附到画布/图层边缘和中心，带参考线
- 翻转图层和翻转画布，水平/垂直

**选区**
- 矩形/椭圆选框、自由/多边形套索、魔棒（按颜色）和对象选择（追踪）
- 选择主体、扩展、收缩、羽化
- 添加/减去选区、移动选区轮廓或选区内像素
- 内容识别填充

**绘画与修饰**
- 画笔：大小、硬度、不透明度、平滑（B/E），Shift 画直线
- 污点修复画笔（内容识别）
- 仿制图章（对齐/不对齐，单图层/所有图层）
- 模糊工具、渐变工具、形状工具（矩形、圆角矩形、椭圆、直线）
- 文字工具（T）：内联多行编辑，字体/大小/颜色/对齐/间距
- 吸管和完整拾色器

**调整和滤镜**
- Camera Raw 滤镜：光线、颜色、曲线、颜色混合器、颜色分级、细节、光学、几何
- 色阶（含自动）、曲线、色相/饱和度、曝光度、渐变映射、颗粒、黑白、色彩平衡、反相
- 高斯/动感模糊、添加杂色、晕影、绽放发光、色调对比、镜头校正、移除背景
- 实时预览，上次滤镜（⌃⌘F）

**画布和文件**
- 标签页管理多个项目
- 搜索命令（⌘F）、切换全屏（F）
- 标尺（⌘R）、参考线、布局网格、吸附
- 裁剪（支持比例 3:4、9:16）
- 画布大小、图像大小、裁剪
- 导入：JPEG、PNG、HEIC、TIFF、SVG、相机 RAW、Photoshop PSD/PSB（8 位 RGB）
- 导出 JPEG 实时预览（⇧⌥⌘S）、合并拷贝
- Photoshop 风格键盘快捷键，可自定义
- 通过 Sparkle 自动更新

**支持 AI 代理**
- `.comp` 项目 = PNG 图层文件夹 + 清单文件；打开的项目在外部修改时实时更新。详见[编写 Compositor 项目](docs/writing-comp-files.md)

### 系统要求
- macOS 26.0 或更高版本，Apple 芯片
- Xcode 26+（从源码构建）

### 构建
打开 `Compositor.xcodeproj`，运行 **Compositor** scheme。

### 致谢

- **原项目**：[Compositor](https://github.com/robbietilton/Compositor)，作者 [Robbie Tilton](https://github.com/robbietilton)
- **中文汉化**：本分支新增完整的简体中文（zh-Hans）本地化，采用 Photoshop 中文版专业术语

### 许可证

MIT — 详见 [LICENSE](LICENSE)。
