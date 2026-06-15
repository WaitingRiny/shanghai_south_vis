# Resonating Echoes (共鸣回响) - Shanghai South Station Data Typography

[English](#english) | [中文说明](#中文说明)

---

## English

**Resonating Echoes** is an interactive, data-driven generative typography installation tailored for the circular departure hall of **Shanghai South Railway Station (上海南站)**. 

By mapping real-time environmental metrics onto displaced concentric circles, the installation visually wiggles and warps typography, drawing public awareness to implicit urban loads.

### 🌟 Key Features
- **Dynamic Data Mapping:** Connects Commuter Density, Noise Level, Air PM2.5, and Wind Velocity to circle spacing, text slice displacements, line thickness, and outward propagation speeds.
- **Bilingual GUI Controls:** Adjust text contents (supports multi-line), font size, weight, wiggling speeds, and color mapping modes on-the-fly.
- **High-Res Poster Export:** Save vertical poster art ($1:\sqrt{2}$ aspect ratio, $1414 \times 2000\text{ px}$) instantly for print.
- **CORS Safe Offline Fallback:** Works directly on local file systems (`file:///`) via embedded datasets.

### 🔗 Live Demo (GitHub Pages)
You can deploy this repository to GitHub Pages to run it online:
1. Go to your repository on GitHub.
2. Select **Settings** -> **Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Choose the `main` branch and `/ (root)` folder, then click **Save**.
5. Your live URL will be active at: `https://WaitingRiny.github.io/shanghai_south_vis/`

---

## 中文说明

**共鸣回响 (Resonating Echoes)** 是一款专为**上海南站**圆形出发大厅设计的交互式城市数据字效投影装置。

本装置提取出发大厅的噪音声级、客流量、空气 PM2.5 与风速风向数据，通过动态重构与位移同心声波线圈，生成具有动态呼吸感的数据排版文字，呼应南站宏伟独特的圆形穹顶钢网架结构，实现视觉艺术、环境声场与地标建筑空间的有机结合。

### 🌟 核心功能
- **数据物理映射:** 
  - 🔊 **噪音声级** $\rightarrow$ 文字扭曲与垂直切片错位（噪音高时，文字内部线圈错落断裂）。
  - 👥 **客流密度** $\rightarrow$ 线条频率与密度（人多时线条紧绷密集，人少时舒缓宽敞）。
  - 😷 **空气 PM2.5** $\rightarrow$ 线条厚度（浓度高时线条变粗、边缘泛红，隐喻空气浑浊）。
  - 🍃 **空气流速** $\rightarrow$ 声波外传流速（风速增加，同心圆环向外发散扩散的速度同步加快）。
- **中英双语控制面板:** 支持多行文本输入、实时字号百分比缩放、字重（Thin 100 到 Black 900）无级调节、声波圆心拖拽定位以及炫彩数据映射。
- **高清 A-Size 海报保存:** 支持一键保存暂停后的竖版海报图像（$1414 \times 2000\text{ px}$），长宽比严格符合 $1:\sqrt{2}$。
- **本地跨域安全回退:** 双击本地 `index.html` 运行网页时，若因浏览器安全策略无法加载外部 CSV，会自动回退载入内置的 24 小时上海南站环境数据集，确保离线即开即用。

### 🔗 在线预览部署
本仓库完全静态，您可一键开启 GitHub Pages 线上预览：
1. 登录 GitHub 进入此项目仓库。
2. 点击右上角 **Settings** 并进入左侧 **Pages** 菜单。
3. 在 **Build and deployment** 下选择 **Deploy from a branch**。
4. Branch 选中 `main` 分支，目录选择 `/ (root)`，点击 **Save** 保存。
5. 保存后稍等 1-2 分钟，即可通过生成的链接访问在线版应用：`https://WaitingRiny.github.io/shanghai_south_vis/`
