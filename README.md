# ⚔️ 草原传说 (Grassland Legend: Worldskills)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Zero Dependencies](https://img.shields.io/badge/Dependencies-0-success?style=for-the-badge)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

> 一款基于纯原生 HTML5 Canvas 打造的硬核动作生存（Vampire Survivors-like）网页游戏。
> **极客美学**：0 外部图片、0 外部音频资源、0 第三方框架。全靠浏览器算力与代码“手搓”的奇迹！

🎮 **[点击这里立即在线试玩！](https://w1839992361.github.io/-Grassland-Legend-/)**

---

## ✨ 游戏特色 (Features)

虽然只是一个单文件网页，但它包含了完整的商业级动作游戏系统：

* **🌪️ 丰富的流派与超武系统**
    * 包含 20+ 种基础技能，自由搭配【冰】、【火】、【雷】、【风】等元素羁绊。
    * 支持符文镶嵌变异，满足特定条件可合成毁天灭地的【超级武器】。
* **🤖 史诗级战局交互**
    * **重装机甲空投**：局内空投可驾驶机甲，接管加特林火控系统，享受物理免伤。
    * **深渊秘境**：地图随机刷新传送门，进入后在 45 秒内极限生存，赢取霸道属性。
    * **动态黑市**：地精商人游荡在地图边缘，只要灵石够，神器直接买。
* **🌦️ 动态世界与环境**
    * **无限生成**：采用 LCG 伪随机算法，无限生成草地、雪原、火山地形。
    * **天气系统**：暴风雪（冰系附带斩杀）、大暴雨（减速玩家并增强雷系）、热浪（怪物加速）。
    * **昼夜交替与光影**：基于 Canvas `destination-out` 的动态全局光照系统。
* **🎵 极客级“纯代码”音效**
    * 不加载任何 MP3 文件，完全使用底层 `Web Audio API` 动态合成街机风音效（射击、升级、怪物爆裂）。
* **📱 全平台适配**
    * 内置双区触控检测与丝滑的虚拟摇杆，PC 端与手机端（微信/手机浏览器）均可完美游玩。

**PC 端控制：**
* `W` `A` `S` `D` 或 `方向键`：移动
* `自动`：索敌与射击
* `Space (空格)`：释放英雄专属大招（如：神风冲刺、圣光治愈）
* `E`：交互（上机甲、进秘境、买东西）
* `F`：主动脱离机甲
* `ESC`：暂停游戏 / 查看战术数据与超武图鉴

**移动端控制：**
* **左半屏长按拖拽**：呼出虚拟摇杆控制移动
* **右半屏点击**：释放大招 / 靠近互动物品时自动交互 / 脱离机甲

## 🛠️ 技术栈与底层架构 (Tech Stack)

本项目是学习 Canvas 高性能渲染和原生 JS 游戏开发的绝佳范例：
* **图形渲染**：`CanvasRenderingContext2D`（包含路径合批、Gradient 降级、Filter 滤镜等压榨性能的操作）。
* **物理碰撞**：自定义 O(1) 复杂度的 **Spatial Hash Grid (空间哈希网格)**，支持同屏 300+ 怪物的流畅碰撞检测。
* **音频合成**：原生 `AudioContext` 震荡器 (Oscillator) 声波合成。
* **UI 架构**：HTML DOM 叠加层 + CSS3 `backdrop-filter` (毛玻璃质感) 与动画。

## 🚀 快速开始 (Quick Start)

因为是零依赖的纯静态页面，运行它不需要任何复杂的环境配置：
1. Clone 或下载本仓库。
2. 双击打开 `index.html`。
3. 即可开始割草！

## 🤝 贡献与参与 (Contributing)
如果你觉得这游戏很酷，欢迎提 Issue 或 Pull Request！你可以尝试添加新的怪物、新的武器配方，或者优化渲染性能。

## 📄 许可 (License)
本项目采用 [MIT License](LICENSE) 开源。享受代码的乐趣吧！
