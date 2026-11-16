# Third-Party Notices / 第三方许可声明

LigSplat is a fork of **Spirula Studio v2026.11.12** by Harry Chen and contributors, licensed under **GNU GPL v3.0**. All upstream copyright and license notices remain applicable. The full GPL-3.0 text is in [LICENSE](LICENSE).

The Windows installer bundles the following components. Their license texts are shipped in the installation directory under `licenses/` and in the corresponding-source archive.

| Component | Version / Notes | License |
|---|---|---|
| Spirula Studio | tag `v2026.11.12`, commit `667e353bca3941303a4d93e93aa8ae3f2c202712` | GPL-3.0 |
| FFmpeg (`avcodec-62`, `avformat-62`, `avfilter-11`, `avutil-60`, `avdevice-62`, `swscale-9`, `swresample-6`, `ffmpeg.exe`, `ffprobe.exe`) | 7.x shared DLL set; GPL and LGPL texts both shipped — the effective combination depends on the build configuration | GPL-3.0 / LGPL-2.1 / LGPL-3.0 (see `licenses/FFmpeg-*.txt`) |
| Node.js runtime (`formats/node.exe`) | bundled for local format conversion only | MIT and bundled dependency licenses (see `licenses/Node.txt`) |
| `@playcanvas/splat-transform` | 3.11.1 | MIT (see its package license) |
| `@adobe/spz` | 0.3.1 | ISC |
| PlayCanvas / `webgpu` | used by the local converter | MIT / respective licenses |
| GLFW | 3.4 | zlib/libpng (see `licenses/GLFW.txt`) |
| Dear ImGui | 1.92.8 | MIT (see `licenses/ImGui.txt`) |
| Vulkan-Headers, apriltag, DINOv3, SAM3 and other upstream deps | as vendored in `LigSplat-0.2.0-source.zip` | see `licenses/spirula/` and each vendored `LICENSE*` |

**Note / 说明**：FFmpeg 的 GPL 与 LGPL 文本同时随包提供，实际构建配置决定适用的许可组合；如需二次分发，请先自行核对 configure 参数与整体许可一致性。/ Both FFmpeg GPL and LGPL texts are provided; the applicable combination depends on the actual build configuration. Verify the configure flags and overall license compatibility before redistributing.

The private report configuration (`report-config.private.json`) and the code-signing private key are **not** part of the corresponding-source archive.
