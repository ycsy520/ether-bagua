🔮 虚空八卦 (Ether Bagua)

"无极生太极，太极生两仪，两仪生四象，四象生八卦。"

虚空八卦 (Ether Bagua) 是一个基于 Web 的增强现实交互装置。它融合了中国古老的道家宇宙观与现代的前沿 WebGL 及计算机视觉技术，创造出一个悬浮于虚空、可被手势操控的赛博法阵。

✨ 核心特性

🌌 纯程序化生成 (Procedural Generation)

摒弃传统静态贴图，所有卦象（阴阳爻）、太极图腾均由 Canvas API 实时计算绘制并生成纹理。

确保在任意分辨率和缩放比例下，纹理边缘依然锐利清晰。

✋ 灵体共鸣交互 (AI Hand Tracking)

集成 Google MediaPipe 视觉模型，无需特殊硬件，仅需普通摄像头。

实时重建 3D 虚拟手骨（赛博义肢），实现与现实手势的 1:1 毫秒级同步。

支持 “悬停即控 (Hover)” 与 “捏合锁定 (Pinch)” 双重交互模式。

⚡️ 物理拟真 (Physics Engine)

模拟真实物体的转动惯量与空气阻力。

实现“意动形随”的流畅手感，松手后卦象会依惯性缓缓流转。

🏮 赛博道家美学 (Cyber-Taoist Aesthetic)

基于 Three.js 的 PBR 材质系统。

引入 UnrealBloom 后处理辉光效果，营造神秘的能量场氛围。

包含动态星尘粒子系统与无限延伸的镜面反射地台。

🛠 技术栈

渲染核心: Three.js (r160)

视觉算法: MediaPipe Tasks Vision

样式框架: Tailwind CSS

开发模式: ES Modules (无构建工具依赖，单文件组件)

🎮 操作指南

启动装置：在现代浏览器（Chrome/Edge/Safari）中打开应用，并允许摄像头权限。

显形：将一只手举起面对摄像头，直到屏幕中同步出现虚拟手骨。

御气（悬停交互）：

将手势光标移动到太极、八卦或六十四卦任意一环上。

圆环高亮即表示建立连接，此时转动手腕/画圆即可带动圆环旋转。

掌控（锁定交互）：

食指与拇指捏合，可强制锁定当前圆环。

此模式下圆环将严格跟随手指坐标，适合进行大幅度、高精度的方位调整。

🚀 本地运行

由于项目使用了 ES Modules 导入方式以及摄像头权限，直接双击打开 .html 文件可能会遇到 CORS 跨域错误。必须使用本地服务器运行。

方法 A: VS Code (推荐)

安装 Live Server 扩展。

右键点击 ether_bagua.html，选择 "Open with Live Server"。

方法 B: Python

如果您安装了 Python，可以在项目目录下运行终端命令：

# Python 3.x
python -m http.server 8000


然后访问 http://localhost:8000/ether_bagua.html

方法 C: Node.js

npx serve .


📜 卦象考据

本项目采用先天八卦 (Pre-Heaven Bagua) 排列，相传为伏羲所定，体现宇宙生成的自然逻辑与阴阳平衡：

乾 (☰)：居南（上），纯阳，主天。

坤 (☷)：居北（下），纯阴，主地。

离 (☲)：居东（左），主火。

坎 (☵)：居西（右），主水。

其余四卦（震、巽、艮、兑）依阴阳消长次序排列，严格遵循先天方位。

Created by the Digital Artificer.
