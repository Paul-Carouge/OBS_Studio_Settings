![Bannière Obs Studio](Screenshots/Banner.png)

# 🇬🇧 English
**Please leave a ⭐ to this repository !**

All theses settings are a base and probably need to be customized to your needs.

## Local Recording Configuration
Use this profile to create high-quality source files, perfect for video editing.

| Section | OBS Parameter | Recommended Setting | Reason |
| :--- | :--- | :--- | :--- |
| **Output (Recording)** | Video Encoder | **NVIDIA NVENC HEVC** | Best efficiency (quality/file size) and supports 10-bit color (`main10`). |
| | Rate Control | **CQP** (Constant Quantization Parameter) | **Guarantees constant quality** by adjusting the bitrate: **no quality loss** and **no artifacts**. |
| | CQ Level | **14-20 (16 recommended)** | Ideal value for visually **lossless** quality. |
| | Recording Format | **MKV** | Safety: protects the file from corruption in case of OBS or system crash. |
| | Preset | **P6: Slow (Best Quality)** | Try P5-P4 if your lagging |
| | Profile | **main10** | For a richer color palette (10-bit) and to prevent banding. |
| **Video** | Base (Canvas) Resolution | **2560x1440** | Native resolution of your monitor. |
| | Output (Scaled) Resolution | **1920x1080-2560x1440** | Records the raw resolution (no scaling). |
| | FPS | **60** | Maximum fluidity. |
| **Advanced** | Color Range | **Full 709.** | For deep blacks and bright whites. |
| | Process Priority | **Normal** | Don't change it!. |

---

## YouTube Streaming Configuration
Use this profile for a stable, fluid, and high-quality live stream, optimized for the platform and your fiber connection.

| Section | OBS Parameter | Recommended Setting | Reason |
| :--- | :--- | :--- | :--- |
| **Output (Streaming)** | Video Encoder | **NVIDIA NVENC H.264** | Required standard for YouTube streaming. |
| | Rate Control | **CBR** (Constant Bitrate) | **Mandatory for a stable stream** without buffering for the viewer. |
| | Bitrate | **12,000 Kbps** | Very high bitrate (change to your connection) for flawless 1080p60 quality, reducing artifacts. |
| | Preset | **P6: Slow (Best Quality)** | Maximizes the quality of the H.264 encoding. |
| | Max B-frames | **2** | Better streaming compatibility and performance. |
| **Video** | Base (Canvas) Resolution | **1920x1080-2560x1440** | Native resolution of your monitor. |
| | Output (Scaled) Resolution | **1920x1080** | Final stream resolution (1080p). |
| | Downscale Filter | **Lanczos (36 Samples)** | Best algorithm for sharp scaling down from 1440p to 1080p. |
| | FPS | **60** | Maximum stream fluidity. |

---

# 🇫🇷 Français
**Ajoute une ⭐ pour ce repository !**

Tous ces paramètres servent de bases et tu va surement devoir les modifiers pour tes besoins.
