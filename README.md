# ATLAS 3D VIEWER

**三维模型检查 · PBR 材质编辑 · 静帧渲染**  
**3D model inspection · PBR material editing · Still-image rendering**

[简体中文](#简体中文) · [English](#english)

**[下载 Windows 安装版 / Download for Windows — v1.2.0](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/releases/download/v1.2.0/ATLAS-3D-Viewer-1.2.0-Setup-x64.exe)**  
[版本说明 / Release notes](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/releases/tag/v1.2.0) · [所有版本 / All releases](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/releases) · [SHA-256](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/releases/download/v1.2.0/ATLAS-3D-Viewer-1.2.0-Setup-x64.exe.sha256)

Windows 10 / 11 · x64 · Version 1.2.0 · 176.43 MiB  
Created by **IKAL ZHUANG**

---

## 简体中文

### ATLAS 是什么？

ATLAS 3D VIEWER 是一款在本机运行的三维模型查看、材质调整与静帧出图工具。你可以在同一个工作区中检查模型结构和 UV、分配 PBR 贴图、调整灯光与镜头，并保存作品展示图片。

适用于三维美术作品检查、游戏资产预览、课堂演示和静帧展示。模型与贴图在本机处理，安装后的查看与渲染工作流可离线使用。

### 主要功能

| 工作区 | 可以做什么 |
| --- | --- |
| 场景 | 查看模型层级、切换可见性、聚焦和单独显示对象，调整位置、旋转与缩放。 |
| 材质 | 编辑基础颜色、粗糙度、金属度、法线、AO、自发光和透明度；批量导入贴图，识别 ARM / ORM / RMA 通道，并手动核对分配。支持材质撤销、重做和单材质 JSON 保存。 |
| UV | 切换网格与 UV 通道，查看棋盘格、线框和面填充，导出当前 UV 视图为 PNG。 |
| 环境 | 使用内置环境或导入 HDR / EXR，调整环境旋转、亮度与背景；配置三点照明。 |
| 动画 | 播放模型自带动画，逐帧查看、拖动时间线，或使用模型转台。 |
| 后期 | 调整曝光、色调映射、白平衡、对比度、饱和度、Bloom 和暗角。 |
| 出图 | 配置透视 / 正交相机、焦距、构图辅助线及输出尺寸，导出 PNG / JPEG；PNG 支持透明背景。 |

提供实时预览与渐进式 GPU 路径追踪，以及 26 种输出尺寸预置，包含常见屏幕尺寸和 150 / 300 PPI 纸张尺寸。界面支持中文、英文、日文、西班牙文、法文和俄文。

### 下载与安装

当前公开版本为 **1.2.0 · Windows 10/11 x64 安装版**。

| 文件 | 用途 |
| --- | --- |
| [ATLAS-3D-Viewer-1.2.0-Setup-x64.exe](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/releases/download/v1.2.0/ATLAS-3D-Viewer-1.2.0-Setup-x64.exe) | 完整安装程序，约 176.43 MiB。 |
| [ATLAS-3D-Viewer-1.2.0-Setup-x64.exe.sha256](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/releases/download/v1.2.0/ATLAS-3D-Viewer-1.2.0-Setup-x64.exe.sha256) | 安装包的 SHA-256 校验文件。 |

1. 下载上表中的安装程序并运行。
2. 按向导选择安装位置、桌面快捷方式及可选的文件关联。
3. 从开始菜单或桌面快捷方式启动 **ATLAS 3D Viewer**。
4. 如需将 ATLAS 设为模型的默认打开程序，请在 Windows“默认应用”中选择。

默认安装到当前用户目录，通常不需要管理员权限。更新前请保存编辑并关闭 ATLAS。卸载可通过 Windows“已安装的应用”完成。

**请使用上面的 EXE 下载链接。** 本仓库提供软件分发与使用说明；GitHub 的 **Code → Download ZIP** 和自动生成的 **Source code (zip)** 只包含本仓库文件，不包含可运行的软件。当前 Release 尚未提供便携 ZIP。

当前安装包未进行代码签名，Windows 可能显示“未知发布者”。请确认文件来自本仓库的正式 Release，并按需核对校验值；不需要关闭系统安全保护。

### 第一次使用

1. 点击“打开模型”，或将模型文件拖入视图。
2. 按 **F** 将模型适配到视图；在“场景”和“UV”中检查结构与 UV。
3. 在“材质”中导入贴图，核对贴图用途和通道分配。
4. 在“环境”中选择照明，在“出图”中调整镜头、构图和分辨率。
5. 选择 PNG 或 JPEG，保存静帧图片。

glTF 的 BIN / 图片以及 OBJ 的 MTL / 图片应与模型保持正确的相对目录关系。**渲染预设不包含模型或材质修改**；需要保留材质设置时，请另外使用单材质 JSON 保存功能。

### 支持的模型格式

| 类别 | 格式与说明 |
| --- | --- |
| 常规模型 | GLB、GLTF、FBX、OBJ、STL、PLY、DAE、3DS、3MF。 |
| 试验性 CAD | STEP / STP、IGES / IGS、BREP。 |
| 试验性 SketchUp | SKP，仅 Windows 桌面版；需要本机 SketchUp 读取库。 |

SKP 导入会查找 SketchUp 2021 及更新版本的本机读取库；本项目实际验证的版本为 **SketchUp 2022**。无需启动 SketchUp，安装包不附带 Trimble 的读取库。不同版本、复杂模型和插件专用数据的兼容性需要分别验证。

MAX、ABC 文件请先在原软件中转换为受支持的格式。

### 快捷键

| 按键 | 功能 |
| --- | --- |
| F | 适配模型到视图 |
| 5 | 切换透视 / 正交投影 |
| G | 显示 / 隐藏地面网格 |
| F11 | 切换全屏 |
| Esc | 退出全屏 |

### 当前范围与限制

- 路径追踪基于 **WebGL GPU**，不是原生 RTX / DXR 后端；首次编译着色器及处理复杂模型可能需要等待。
- 动画和转台使用实时模式；当前导出为静帧图片，不提供视频导出。
- 输出尺寸为每边 64–8192 像素、总计不超过 24 MP，同时受显卡能力限制。
- 路径追踪贴图图集上限为 2K；增加采样数不会提升超过此上限的贴图细节。
- 景深仅用于透视路径追踪。透明 PNG 会隐藏地面，不提供独立的透明阴影或反射层。
- 文件格式支持不代表所有第三方扩展、约束、超大资源或渲染器专用材质都能完整还原。

### 反馈问题

请通过 [GitHub Issues](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/issues) 提交问题，尽量附上软件版本、Windows 版本、显卡型号、模型格式、复现步骤和截图。模型文件仅在你有权公开分享时提供。

---

## English

### What is ATLAS?

ATLAS 3D VIEWER is a local application for viewing 3D models, editing PBR materials, and rendering still images. Inspect scene structure and UVs, assign texture maps, adjust lighting and camera settings, and export presentation images from one workspace.

It is designed for 3D artwork review, game-asset previews, classroom demonstrations, and still-image presentation. Models and textures are processed on your computer; viewing and rendering work offline after installation.

### Features

| Workspace | What you can do |
| --- | --- |
| Scene | Inspect the hierarchy, control visibility, focus or isolate objects, and adjust position, rotation, and scale. |
| Materials | Edit base color, roughness, metalness, normals, AO, emission, and transparency. Import texture sets, review ARM / ORM / RMA channel assignments, undo or redo edits, and save individual materials as JSON. |
| UV | Select meshes and UV channels, inspect checkerboard and wireframe views, and export the current UV view as PNG. |
| Environment | Use built-in environments or load HDR / EXR files; adjust rotation, intensity, backgrounds, and three-point lighting. |
| Animation | Play embedded animations, step through frames, scrub the timeline, or use the turntable. |
| Post-processing | Adjust exposure, tone mapping, white balance, contrast, saturation, bloom, and vignette. |
| Render | Set perspective or orthographic cameras, focal length, composition guides, and image dimensions. Export PNG / JPEG, including transparent PNG. |

The viewer includes real-time preview, progressive GPU path tracing, and 26 output-size presets covering common screen formats and paper sizes at 150 / 300 PPI. Interface languages include Chinese, English, Japanese, Spanish, French, and Russian.

### Download and install

The current public release is **1.2.0 for Windows 10/11 x64**.

| File | Purpose |
| --- | --- |
| [Windows installer — ATLAS-3D-Viewer-1.2.0-Setup-x64.exe](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/releases/download/v1.2.0/ATLAS-3D-Viewer-1.2.0-Setup-x64.exe) | Complete installer, approximately 176.43 MiB. |
| [SHA-256 checksum](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/releases/download/v1.2.0/ATLAS-3D-Viewer-1.2.0-Setup-x64.exe.sha256) | Verify the installer download. |

1. Download and run the installer.
2. Choose the installation location, desktop shortcut, and optional file associations.
3. Launch **ATLAS 3D Viewer** from the Start menu or desktop.
4. To make ATLAS the default model viewer, select it in Windows **Default apps** settings.

The default installation is per-user and normally does not require administrator privileges. Save your work and close ATLAS before updating. Uninstall through Windows **Installed apps**.

**Download the EXE linked above.** This repository hosts distribution information and documentation. **Code → Download ZIP** and GitHub's automatic **Source code (zip)** contain repository files, not the application. A portable ZIP is not currently attached to this release.

The installer is currently unsigned, so Windows may display an unknown-publisher message. Confirm that it came from this repository's official Release and verify its checksum if needed; do not disable system security protections.

### Quick start

1. Choose **Open Model** or drag a model into the viewer.
2. Press **F** to frame the model, then inspect it in Scene and UV.
3. Import texture maps in Materials and review their roles and channels.
4. Set up Environment lighting and choose camera, composition, and image dimensions in Render.
5. Export a PNG or JPEG still image.

Keep glTF BIN / image files and OBJ MTL / image files in the directory structure expected by the model. **Render presets do not include the model or material edits.** Save individual materials separately as JSON when you need to retain their settings.

### Supported formats

| Category | Formats and scope |
| --- | --- |
| Model import | GLB, GLTF, FBX, OBJ, STL, PLY, DAE, 3DS, 3MF. |
| Experimental CAD | STEP / STP, IGES / IGS, BREP. |
| Experimental SketchUp | SKP, Windows desktop only; requires a local SketchUp reading library. |

SKP import searches for reading libraries from SketchUp 2021 or later. **SketchUp 2022 is the version tested in this project.** SketchUp does not need to be running, and Trimble's libraries are not included in the installer. Other versions, complex projects, and plug-in data require separate compatibility checks.

Convert MAX and ABC files in their original software before importing.

### Keyboard shortcuts

| Key | Action |
| --- | --- |
| F | Frame the model |
| 5 | Toggle perspective / orthographic projection |
| G | Toggle the ground grid |
| F11 | Toggle fullscreen |
| Esc | Exit fullscreen |

### Current scope and limitations

- Path tracing uses **WebGL GPU rendering**, not a native RTX / DXR backend. Initial shader compilation and complex models may take time.
- Animation and turntable playback use real-time rendering. Export is limited to still images; video export is not included.
- Output dimensions range from 64 to 8192 pixels per side, with a 24-megapixel total limit and additional GPU-dependent limits.
- The path-tracing texture atlas is limited to 2K. More samples do not recover texture detail beyond that limit.
- Depth of field is available only in perspective path tracing. Transparent PNG hides the ground and does not provide separate transparent shadow or reflection layers.
- Format support does not guarantee full reproduction of every extension, constraint, large asset, or renderer-specific material.

### Report an issue

Use [GitHub Issues](https://github.com/vikrante/ATLAS-3D-VIEWER-Downloads/issues). Include the application version, Windows version, GPU model, file format, steps to reproduce, and screenshots when available. Only attach models that you have permission to share publicly.

---

## SHA-256 · 下载校验 / Download verification

在下载目录中打开 PowerShell，运行以下命令，将结果与同版本的 `.sha256` 文件比较。  
Open PowerShell in your download folder, run the command below, and compare the result with the matching `.sha256` file.

```powershell
Get-FileHash -LiteralPath '.\ATLAS-3D-Viewer-1.2.0-Setup-x64.exe' -Algorithm SHA256
```

**v1.2.0 installer SHA-256:**

```text
3E105151A38898941D1CD078B87EBEFFAA06750350274BE6A68EEFB29F4AB76E
```

本仓库用于 ATLAS 3D VIEWER 的软件下载与用户文档，不包含应用源码。第三方组件声明随安装包提供。  
This repository provides ATLAS 3D VIEWER downloads and user documentation, not the application source code. Third-party notices are included with the application.

