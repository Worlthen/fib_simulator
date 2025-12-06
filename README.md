# 🔬 FIB 虚拟仿真系统

基于 WebGL 的聚焦离子束 (Focused Ion Beam) 实时仿真平台，采用 Yamamura 溅射模型，支持多层材料结构。

## 🌐 在线演示

**[点击这里体验 →](https://worlthen.github.io/fib_simulator/)**

## 📦 包含工具

| 版本 | 功能 | 适用场景 |
|------|------|----------|
| ⚡ 基础版 | 手动加工、参数调节、3D 可视化 | 快速体验 |
| 🎓 教学版 | 预设图案、自动铣削、深度剖面图 | 课堂演示 |
| 🔬 科研版 | 多层材料、剂量计算、STL 导出 | 科研分析 |

## 🚀 快速部署

### GitHub Pages (推荐)

1. Fork 本仓库或下载所有文件
2. 进入仓库 Settings → Pages
3. Source 选择 `main` 分支
4. 保存后等待几分钟即可访问

### 本地运行

```bash
# 使用 Python
python -m http.server 8000

# 或使用 Node.js
npx serve .
```

然后访问 `http://localhost:8000`

## 🔬 技术特性

- **Yamamura 溅射模型** - 真实模拟角度依赖的溅射产额
- **GPGPU 计算** - 使用 WebGL 着色器进行高性能并行计算
- **多层材料** - 支持 Si、SiO₂、Au、Pt、Cu 等多种材料
- **实时分析** - 剂量、深度、体积实时计算
- **数据导出** - STL 3D 模型 / JSON 数据导出

## 📁 文件结构

```
fib-simulator/
├── index.html          # 首页
├── FIB.html            # 基础仿真版
├── FIB_Education.html  # 教学演示版
├── FIB_Research.html   # 科研工具版
└── README.md           # 说明文档
```

## 🎮 操作说明

| 操作 | 功能 |
|------|------|
| 左键拖动 | 进行 FIB 加工 |
| 右键拖动 | 旋转视角 |
| 滚轮 | 缩放视图 |

## 📖 FIB 简介

聚焦离子束 (FIB) 是一种利用聚焦的离子束（通常是 Ga⁺）对材料进行纳米级加工的技术。主要应用：

- 🔍 半导体失效分析
- 🔬 TEM 样品制备
- ✂️ 微纳加工
- 📸 离子束成像

## 🛠️ 技术栈

- [Three.js](https://threejs.org/) - 3D 渲染引擎
- WebGL 2.0 - GPU 加速计算
- GLSL 着色器 - GPGPU 仿真

## 📄 许可

MIT License - 仅供学习交流使用

---

⭐ 如果觉得有用，欢迎 Star！
