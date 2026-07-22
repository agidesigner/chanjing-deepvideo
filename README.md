<div align="center">

# 蝉镜AI DeepVideo · JoggAI DeepVideo

**把普通视频转换为时序一致的可视化深度视频**  
**Turn regular footage into temporally consistent depth video — locally on your Mac**

[下载最新版 / Download Latest](https://github.com/agidesigner/chanjing-deepvideo/releases/latest) · [中文](#中文) · [English](#english)

</div>

> 此仓库仅发布安装包和版本说明，不包含应用源代码。  
> This repository distributes installers and release notes only. Application source code is not included.

---

## 中文

### 下载

- **macOS（Apple Silicon）**：[前往 GitHub Releases 下载最新 DMG](https://github.com/agidesigner/chanjing-deepvideo/releases/latest)
- **Windows**：正在开发中，发布后会在本仓库提供下载。

蝉镜AI DeepVideo 是一款面向创作者的本地视频深度生成工具。选择视频后，应用会在 Mac 上逐帧估计画面深度，生成具有稳定时序效果的彩色深度视频。Small 模型已包含在安装包内，安装完成后无需再次下载模型。

### 核心功能

- **本地 AI 处理**：视频和生成结果保留在本机，不上传到云端。
- **时序一致的深度估计**：减少逐帧处理常见的闪烁，适合连续视频素材。
- **模型随 App 内置**：安装后即可使用，不需要配置 Python、Conda 或命令行环境。
- **可感知的生成进度**：显示处理阶段、帧数、百分比、已用时间和预计剩余时间。
- **应用内结果预览**：生成后可直接播放深度视频，并一键打开输出文件夹。
- **中英文界面**：中文系统显示简体中文，其他系统语言显示英文。
- **应用内更新提醒**：发现新版本时显示下载入口，也可从 macOS 应用菜单手动检查更新。

### 适用场景

- **三维视差与空间动画**：为照片动画、镜头推进和 2.5D 视觉效果提供深度参考。
- **影视合成与特效**：辅助景深、雾效、光照、遮挡和分层合成。
- **深度感知剪辑**：为前后景分离、区域蒙版和风格化处理提供基础素材。
- **AI 视频创作**：将深度视频用于 ControlNet、生成式视频及其他视觉工作流。
- **快速预演**：无需搭建开发环境，快速判断一段素材的空间层次与深度稳定性。

> 当前版本生成的是**相对深度可视化**，不代表真实世界的绝对距离或测量结果。

### 系统要求

- Apple Silicon Mac：M1 或更新芯片
- macOS 12.3 或更高版本
- 建议至少 8 GB 内存；高质量模式建议 16 GB 或更多
- 输入格式：常见 MP4、MOV、M4V、AVI、MKV 视频（推荐 H.264 MP4/MOV）

### 安装与使用

1. 从 [Releases](https://github.com/agidesigner/chanjing-deepvideo/releases/latest) 下载 `.dmg`。
2. 打开 DMG，将“蝉镜 DeepVideo”拖入“应用程序”。
3. 首次启动若 macOS 显示安全提示，请在 Finder 中右键应用并选择“打开”。
4. 选择输入视频和输出文件夹，选择生成质量，然后开始处理。
5. 完成后在应用内预览，或点击“打开输出文件夹”。

每次生成会输出：

- `原文件名_src.mp4`：标准化后的源视频
- `原文件名_depth.mp4`：彩色深度视频

更多 AI 视频创作能力，请访问 [蝉镜官网](https://chanjing.cc/?source=deepvideo)。

---

## English

### Download

- **macOS (Apple Silicon)**: [Download the latest DMG from GitHub Releases](https://github.com/agidesigner/chanjing-deepvideo/releases/latest)
- **Windows**: In development. The installer will be published in this repository when it is ready.

JoggAI DeepVideo is a local video-depth tool for creators. It estimates depth frame by frame on your Mac and produces a colorized depth video with consistent motion over time. The Small model is bundled with the application, so no separate model download or Python setup is required after installation.

### Features

- **Local AI processing**: Input videos and generated files stay on your Mac and are not uploaded to the cloud.
- **Temporally consistent depth**: Reduces frame-to-frame flicker for continuous footage.
- **Bundled model**: No Python, Conda, command line, or additional model download is required.
- **Detailed progress**: See the current stage, processed frames, percentage, elapsed time, and estimated time remaining.
- **In-app preview**: Play the generated depth video and open its output folder in one click.
- **Bilingual interface**: Simplified Chinese on Chinese systems and English for all other system languages.
- **Update notifications**: Get a download shortcut when a new release is available, or check manually from the macOS application menu.

### Use Cases

- **3D parallax and spatial animation**: Create depth-driven camera moves and 2.5D effects.
- **Compositing and visual effects**: Support depth of field, fog, lighting, occlusion, and layered composites.
- **Depth-aware editing**: Build foreground/background masks and stylized effects from spatial structure.
- **Generative video workflows**: Use depth output with ControlNet, generative video tools, and other creative pipelines.
- **Fast previs**: Evaluate the spatial structure and temporal stability of footage without setting up a development environment.

> The app produces a **relative depth visualization**. It is not an absolute real-world distance measurement.

### Requirements

- Apple Silicon Mac with an M1 chip or newer
- macOS 12.3 or later
- 8 GB memory minimum recommended; 16 GB or more recommended for High Quality mode
- Common MP4, MOV, M4V, AVI, and MKV inputs (H.264 MP4/MOV recommended)

### Install and Use

1. Download the `.dmg` from [Releases](https://github.com/agidesigner/chanjing-deepvideo/releases/latest).
2. Open the DMG and drag “蝉镜 DeepVideo” to Applications.
3. If macOS displays a security warning on first launch, Control-click the app in Finder and choose Open.
4. Choose an input video and output folder, select the quality, and start processing.
5. Preview the result in the app or choose Open Output Folder.

Each run creates:

- `original-name_src.mp4`: normalized source video
- `original-name_depth.mp4`: colorized depth video

For more AI video creation tools, visit [JoggAI](https://jogg.ai/?source=deepvideo).

---

### Technology and Distribution Notice

Depth estimation is powered by [Video Depth Anything](https://github.com/DepthAnything/Video-Depth-Anything). Third-party components and models remain subject to their respective licenses. The DeepVideo application is distributed as proprietary software; downloading or using the installer does not grant access to its source code.

