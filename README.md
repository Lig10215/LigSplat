# LigSplat 0.2.0-preview · 软件说明（中英文对照）
# LigSplat 0.2.0-preview · Software Description (Bilingual)

> ## 立即下载 / Download
>
> ### [点击直接下载 LigSplat 安装包（.exe）](https://github.com/Lig10215/LigSplat/releases/latest/download/LigSplat-Setup-0.2.0-win64.exe)
>
> 当前 `v0.2.0-preview` · 200 MiB · Windows 10/11 64 位。**点击上方链接即开始下载，无需再进入 Releases 页面。**
>
> ### [Click to download the LigSplat installer (.exe)](https://github.com/Lig10215/LigSplat/releases/latest/download/LigSplat-Setup-0.2.0-win64.exe)
>
> Current `v0.2.0-preview` · 200 MiB · Windows 10/11 64-bit. **The link above downloads the installer directly — no Releases page in between.**
>
> 其他文件：[完整对应源码 ZIP](https://github.com/Lig10215/LigSplat/releases/latest/download/LigSplat-0.2.0-source.zip) · [SHA256 校验清单](https://github.com/Lig10215/LigSplat/releases/latest/download/SHA256SUMS-0.2.0.txt) · [最新版 Release 页面](https://github.com/Lig10215/LigSplat/releases/latest)（含全部文件与历史版本）
> Other files: [corresponding source ZIP](https://github.com/Lig10215/LigSplat/releases/latest/download/LigSplat-0.2.0-source.zip) · [SHA-256 manifest](https://github.com/Lig10215/LigSplat/releases/latest/download/SHA256SUMS-0.2.0.txt) · [latest Release page](https://github.com/Lig10215/LigSplat/releases/latest) (all files and older builds)
>
> 说明：直链固定指向「最新版中同名附件」，不写死版本 tag；若将来安装包改名，请从上面的 Release 页面下载。文件哈希与校验方法见第 2 节。
> Note: the direct link always resolves to the same-named asset in the **latest** Release, without pinning a tag. If the installer is ever renamed, use the Release page above. Hashes and verification steps are in §2.

> 版本 / Version：`0.2.0-preview`（2026-11-17）
> 作者 / Author：Lig10215
> 项目地址 / Repository：https://github.com/Lig10215/LigSplat
> 本文逐节「中文 → English」对照 / Each section is given in Chinese, then in English.

---

## 1. 这是什么 / What it is

**中文**

LigSplat 是面向 **Windows x64** 的本地 3D Gaussian Splatting（3DGS）工作站，基于 Harry Chen 及上游贡献者的 **Spirula Studio `v2026.11.12`**（commit `667e353bca3941303a4d93e93aa8ae3f2c202712`，GPL-3.0）本地分支，以**原生 C++ / Vulkan 单体程序**实现。它把「照片或视频 → SfM 相机重建 → 3DGS 训练 → 预览与清理 → 多格式导出」串在同一套桌面界面里。重建、训练、渲染与格式转换全部在本机 CPU/GPU 完成，**核心流程不需要云端账号或 Python / CUDA / PyTorch 运行环境**。随包附带 FFmpeg 与 Node + `@playcanvas/splat-transform 3.11.1`，仅用于本地视频处理和模型格式转换。

**English**

LigSplat is a **local 3D Gaussian Splatting (3DGS) workstation for Windows x64**, implemented as a **native C++ / Vulkan application** from a local fork of **Spirula Studio `v2026.11.12`** (commit `667e353bca3941303a4d93e93aa8ae3f2c202712`, GPL-3.0) by Harry Chen and upstream contributors. It brings "photos or video → SfM camera reconstruction → 3DGS training → preview and cleanup → multi-format export" into one desktop interface. Reconstruction, training, rendering and conversion all run on the local CPU/GPU; the core workflow requires no cloud account or Python/CUDA/PyTorch runtime. FFmpeg and Node + `@playcanvas/splat-transform 3.11.1` are bundled for local video handling and model-format conversion only.

---

## 2. 下载与完整性校验 / Download and integrity verification

**中文**

下表中的**文件名都是直接下载链接，点击即可开始下载**（无需进入 Releases 页面）。v0.2.0 提供三个文件：Windows 安装包、完整对应源码包、校验清单。全部文件与历史版本见 [Releases 最新版](https://github.com/Lig10215/LigSplat/releases/latest)。下载后用 `certutil -hashfile <文件名> SHA256` 核对哈希，与 `SHA256SUMS-0.2.0.txt` 比对。

**English**

**Every filename below is a direct download link — one click starts the download**, with no Releases page in between. v0.2.0 ships three files: the Windows installer, the complete corresponding-source archive, and a checksum manifest. All files and older builds are on the [latest Release](https://github.com/Lig10215/LigSplat/releases/latest). Verify with `certutil -hashfile <filename> SHA256` and compare against `SHA256SUMS-0.2.0.txt`.

| 文件 / File（点击下载 / click to download） | 大小 / Size | SHA-256 |
|---|---|---|
| [`LigSplat-Setup-0.2.0-win64.exe`](https://github.com/Lig10215/LigSplat/releases/latest/download/LigSplat-Setup-0.2.0-win64.exe) | 209,698,192 B (200.0 MiB) | `c8d7712c750047308d815b1df7f2a50433570327bc08759ee3f9da99fc2cac77` |
| [`LigSplat-0.2.0-source.zip`](https://github.com/Lig10215/LigSplat/releases/latest/download/LigSplat-0.2.0-source.zip) | 21,413,832 B (20.4 MiB) | `53a9c6a51285f4bb473b881fcd92c38dc8dd9ad157e068daf9761c3b92a9526c` |
| [`SHA256SUMS-0.2.0.txt`](https://github.com/Lig10215/LigSplat/releases/latest/download/SHA256SUMS-0.2.0.txt) | 277 B | — |

### 版本说明 / Version notes

**中文**

| 版本 / Version | 状态 / Status | 说明 / Notes |
|---|---|---|
| **v0.2.0-preview（最新版，推荐）** | 当前维护版本 | 新增「补拍与派生任务」（OOOSplat 项目 + 新影像 → 独立派生目录）、每 250 步训练检查点与暂停/继续恢复，并完成真实视频短流程与中断恢复实测。**普通用户请只用文档顶部的「最新版」直链下载**：[LigSplat-Setup-0.2.0-win64.exe](https://github.com/Lig10215/LigSplat/releases/latest/download/LigSplat-Setup-0.2.0-win64.exe)。 |

**English**

| Version | Status | Notes |
|---|---|---|
| **v0.2.0-preview (latest, recommended)** | currently maintained | Adds Reshoot & derived tasks (OOOSplat project + new imagery → separate derived directory), training checkpoints every 250 steps with pause/resume, plus validation on a real short video and an interrupted-resume run. **Most users should only use the "latest" direct link at the top of this document**: [LigSplat-Setup-0.2.0-win64.exe](https://github.com/Lig10215/LigSplat/releases/latest/download/LigSplat-Setup-0.2.0-win64.exe). |

**引导原则：普通用户一律使用最新版 v0.2.0。** / **Guidance: always start with the latest v0.2.0.**

---

## 3. 系统要求与安装 / Requirements and installation

**中文**

- Windows 10 / 11 **64 位**，需显卡厂商提供的 **Vulkan 驱动**；已在 **AMD Radeon RX 9070 XT 16 GB** 上验证，其他显卡与 Windows 10 尚未逐机验证。
- 运行安装包即可，**每用户安装**，默认目录 `%LOCALAPPDATA%\Programs\LigSplat`；桌面生成 `LigSplat` 快捷方式（启动参数 `--lang zh-hans`）。
- **不覆盖 OOOSplat**，不修改已有模型或其安装目录；卸载清单只含程序自身文件，派生任务与模型数据不会被删除。
- 安装包与程序使用 **Lig10215 自签名证书**，不是公众信任的 CA 代码签名证书，且**没有 RFC3161 时间戳**。Windows / SmartScreen 可能提示「未知发布者」；安装程序不会自动修改系统证书信任库。请自行核对上一节哈希后再决定是否运行。

**English**

- **64-bit** Windows 10 / 11 with a vendor-supplied **Vulkan driver**. Validated on an **AMD Radeon RX 9070 XT 16 GB**; other GPUs and Windows 10 have not been verified machine by machine.
- Run the installer for a **per-user installation** into `%LOCALAPPDATA%\Programs\LigSplat`. A `LigSplat` desktop shortcut is created (launch argument `--lang zh-hans`).
- It **does not overwrite OOOSplat** and does not modify existing models or their installation directories. The uninstall manifest contains only program files; derived tasks and model data are never removed.
- The installer and executable are signed with a **self-signed Lig10215 certificate**, not a publicly trusted CA code-signing certificate, and carry **no RFC3161 timestamp**. Windows / SmartScreen may report an "unknown publisher"; the installer does not modify the system trust store. Verify the hashes above before deciding to run it.

---

## 4. 主要功能 / Features

**中文**

| 模块 / Module | 说明 / Description |
|---|---|
| 本地生成 / Local generation | 从照片、视频或素材目录创建数据集，设置抽帧数量；SIFT 特征提取、图像匹配、SfM 重建与 BA 均在本机运行；检查注册数量、重投影误差与相机分布后开始 3DGS 训练；训练检查点支持续训，批处理页可串联数据准备、重建与训练。 |
| 补拍与派生任务 / Reshoot & derived tasks | 读取原 OOOSplat 项目（schema 1–9）的 `project.json`、新增视频或图片目录，在**独立派生目录**中保存快照、注册结果、检查点与 `final.ply`；原项目只读、不写入、不移动。 |
| 预览与游览 / Preview & navigation | 自由游览 / 第一人称模式（W/S 前后、A/D 左右、E 上升、Q 下降，1–10 档速度）；晴天、暴雨、暴雪、黑夜等天气预览与强度调节。 |
| 清理与编辑 / Cleanup & editing | 基于空间密度、连通分量、尺度与无效数据判据自检并清理漂浮颗粒；清理**可撤销**，通过「另存为」保留结果，原始文件不变。 |
| 格式转换 / Format conversion | 打开 PLY、压缩 PLY、SPZ、SOG、SPLAT、KSPLAT；另存 PLY、压缩 PLY、SPZ v4、SOG、离线 HTML。转换由随包的 PlayCanvas 工具在**本机 CPU** 执行。 |
| 导出 / Export | 原生渲染界面支持相机路径、照片与视频导出。 |

**English**

| Module | Description |
|---|---|
| Local generation | Create a dataset from photos, video or an asset folder and set frame extraction. SIFT features, image matching, SfM reconstruction and bundle adjustment all run locally. Start 3DGS training after reviewing registered image count, reprojection error and camera distribution; training checkpoints support resuming, and the batch page chains data prep, reconstruction and training. |
| Reshoot & derived tasks | Read an original OOOSplat project (schema 1–9) `project.json` plus new video or image folders, and save snapshots, registration results, checkpoints and `final.ply` in a **separate derived directory**. The original project is read-only: it is never written to or moved. |
| Preview & navigation | Free-flight / first-person modes (W/S forward-back, A/D left-right, E up, Q down, 10 speed levels); weather previews (clear, heavy rain, heavy snow, night) with intensity control. |
| Cleanup & editing | Detect and remove floating particles using spatial density, connected components, scale and invalid-data criteria. Cleanup is **undoable**; use "Save As" to keep the result, leaving the original untouched. |
| Format conversion | Open PLY, compressed PLY, SPZ, SOG, SPLAT, KSPLAT; save as PLY, compressed PLY, SPZ v4, SOG or offline HTML. Conversion runs on the **local CPU** via the bundled PlayCanvas tooling. |
| Export | The native viewer supports camera paths, photos and video export. |

---

## 5. 0.2.0 新增内容 / What is new in 0.2.0

**中文**

- **补拍与派生任务**：支持选择 OOOSplat 项目、新视频或图片目录，创建独立派生任务；快照包含已注册原画面、原相机模型、来源元数据与已有删除掩码，每个阶段保存哈希清单。不同盘符、中文与空格路径已实测，拒绝大小写变体造成的源目录嵌套。
- **联合重建门槛**：新增画面必须与至少 3 张原画面注册到**同一重建分量**才允许开始本地 Vulkan 训练；无共同分量时停在重建阶段，不训练、不假报成功。本版本使用新旧画面联合重建并重新训练，**会产生新坐标系**。
- **暂停与恢复**：暂停会停止任务持有的子进程；继续时先核验各阶段文件再复用结果。训练每 **250 步**保存参数与优化器检查点，异常退出后可从最近完整检查点恢复，未保存的少量步数需要重算。已完成任务点击「继续」只核验、不重复计算。软件记住最近任务路径并显示磁盘中的阶段状态。

本轮实测包括：31 张原画面 + 16 张新画面联合注册、中文带空格 MP4 视频全流程、250 步检查点中断恢复到 3000 步、GUI 全流程、清理撤销另存（5000 → 4000 点）、SPZ / SOG / 压缩 PLY 往返、天气切换、导航与 Vulkan fp64 CAS 数值测试。300 步 GUI 补拍导出 99,997 点，恢复后 3000 步导出 321,657 点，数值均有限。这是**短片段功能验证**，不是完整成品质量或空地绝对坐标精度验收。

**English**

- **Reshoot & derived tasks**: select an OOOSplat project plus new video or image folders to create an independent derived task. Snapshots include registered original frames, the original camera model, provenance metadata and existing deletion masks, with a hash manifest per stage. Cross-drive, Chinese and space-containing paths were tested; nested source directories caused by case variants are rejected.
- **Joint-reconstruction gate**: new frames must be registered into the **same reconstruction component** as at least 3 original frames before local Vulkan training may start. Without a shared component, the run stops at reconstruction — no training and no false success. This version jointly reconstructs old and new frames and retrains, so **a new coordinate system is produced**.
- **Pause and resume**: pausing stops the child processes owned by the task; resuming verifies every stage's files before reusing results. Full parameter and optimizer checkpoints are saved every **250 steps**; after an abnormal exit the run resumes from the latest complete checkpoint, and the few unsaved steps are recomputed. Clicking "Continue" on a finished task only verifies results without recomputation. The app remembers the most recent task path and shows on-disk stage status.

Validation this round covered joint registration of 31 original + 16 new frames, a full pipeline on an MP4 with Chinese and spaces in its path, interruption at the 250-step checkpoint and resume to 3000 steps, the full GUI flow, cleanup/undo/save-as (5000 → 4000 points), SPZ / SOG / compressed-PLY round trips, weather switching, navigation, and Vulkan fp64 CAS numerical tests. The 300-step GUI reshoot exported 99,997 points and the resumed 3000-step run exported 321,657 points, all finite. These are **short-clip functional checks**, not acceptance of finished production quality or absolute air-ground coordinate accuracy.

---

## 6. 已知限制 / Known limitations

**中文**

- 这是**可运行的预览版**，不是 OOOSplat 全功能等价替代品。固定原相机的增量注册、维持原坐标的热启动、Brush 优化器迁移、把原高斯删除索引自动映射到新训练结果，以及 OOOSplat 专用 ERP / GPS / 全部补拍分支**尚未实现**。
- 天气是**预览叠加与色调模拟**，不是物理重光照，也不生成可导出的积雪几何。
- 漂浮颗粒清理 10 档累计至少删除原始点数的 20%；模型本来干净时**可能误删有效细节**，通用算法无法保证区分云雾、植被、细线与真实独立物体，请多视角检查后再另存。
- 压缩格式（SPZ / SOG / 压缩 PLY）为**有损转换**，完整参数请保留原始 PLY。
- **没有重叠的空地素材不能仅凭一个按钮推断出真实坐标**，应补充共同视角或控制信息。
- 批处理、网格、全景与相机路径导出等功能的全部参数组合**未做穷举回归**；上表即本轮实际执行范围。

**English**

- This is a **working preview**, not a full-featured OOOSplat replacement. Fixed-original-camera incremental registration, warm starts preserving the original coordinate frame, Brush optimizer migration, automatic mapping of original Gaussian deletion indices onto new training results, and OOOSplat-specific ERP / GPS / all reshoot branches are **not implemented**.
- Weather is a **preview overlay and tone simulation**, not physically based relighting, and does not generate exportable snow geometry.
- The 10 cleanup levels remove at least 20% of the original points in total; on an already clean model this **may delete valid detail**. A generic algorithm cannot reliably distinguish clouds, foliage, thin wires and genuinely separate objects — inspect from several angles before saving.
- Compressed formats (SPZ / SOG / compressed PLY) are **lossy**; keep the original PLY for full parameters.
- **Air-ground captures without overlap cannot be placed in true coordinates by pressing a single button**; add shared viewpoints or control information.
- Not every parameter combination of batch processing, meshing, panorama and camera-path export has been regression-tested; the table above is the exact scope executed this round.

---

## 7. 隐私与网络行为 / Privacy and network behaviour

**中文**

- 重建、训练、预览、清理与格式转换**全部在本地**完成。程序不上传照片、视频、模型或源代码文件。
- 本软件不含自动遥测；如需反馈问题，请通过本仓库 Issues 或邮件联系。

**English**

- Reconstruction, training, preview, cleanup and conversion all happen **locally**. The program does not upload photos, videos, models or source files.
- There is no automatic telemetry; for feedback, use this repository's Issues or contact the author by email.

---

## 8. 许可证与对应源码 / License and corresponding source

**中文**

LigSplat 基于 **Spirula Studio v2026.11.12**（Harry Chen 及贡献者，**GPL-3.0**）的本地分支，本仓库以 [GNU GPL v3.0](LICENSE) 授权，保留全部上游版权与许可声明。依照 GPL-3.0，**每个 Release 都随附完整对应源码**：`LigSplat-0.2.0-source.zip` 包含本地修改、构建脚本与打包脚本，可用 `BUILDING.md` 所述工具链（Visual Studio 2022 C++ 生成工具、CMake、Ninja、Vulkan SDK、Slang 2026.12.0.1）重建，构建选项 `-DSS_BACKEND=vulkan -DSS_BUILD_SAM=OFF -DSS_ENABLE_PATENTED=OFF -DSS_SFM_F64_CAS=ON`。随包第三方组件（FFmpeg GPL/LGPL、GLFW、ImGui、Node、PlayCanvas、@adobe/spz、Vulkan-Headers 等）的声明见 [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md)，并随安装包放在 `licenses/` 目录。

**English**

LigSplat is a local fork of **Spirula Studio v2026.11.12** (Harry Chen and contributors, **GPL-3.0**); this repository is licensed under the [GNU GPL v3.0](LICENSE) and preserves all upstream copyright and license notices. Per GPL-3.0, **every Release ships the complete corresponding source**: `LigSplat-0.2.0-source.zip` contains the local modifications, build scripts and packaging scripts, and can be rebuilt with the toolchain described in `BUILDING.md` (Visual Studio 2022 C++ Build Tools, CMake, Ninja, Vulkan SDK, Slang 2026.12.0.1) using `-DSS_BACKEND=vulkan -DSS_BUILD_SAM=OFF -DSS_ENABLE_PATENTED=OFF -DSS_SFM_F64_CAS=ON`. Notices for bundled third-party components (FFmpeg GPL/LGPL, GLFW, ImGui, Node, PlayCanvas, @adobe/spz, Vulkan-Headers and others) are listed in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) and shipped in the installer's `licenses/` directory.

---

## 9. 作者与联系 / Author and contact

**中文**

作者 **Lig10215** · 联系：qliguangshengq@qq.com · 项目：https://github.com/Lig10215/LigSplat
上游 / Upstream：https://github.com/harry7557558/spirula-studio
问题反馈建议使用本仓库 Issues。

**English**

Author **Lig10215** · Contact: qliguangshengq@qq.com · Repository: https://github.com/Lig10215/LigSplat
Upstream: https://github.com/harry7557558/spirula-studio
Please use this repository's Issues for feedback.
