# 行程问题可视化工具 - 模块1

> 直线往返相遇问题可视化演示工具

## ✨ 功能特点

- **4次相遇快照** - 自动记录每次相遇的完整轨迹
- **轨迹自动下移** - 折返时轨迹自动向下偏移，避免重叠
- **实时动画 + 历史快照** - 双区域展示，清晰对比
- **固定标签系统** - 1s, 2s, 5s, 7s
- **Notion风格设计** - 温暖米白色调，简洁优雅
- **纯HTML + Canvas** - 零依赖，单文件运行

## 🚀 快速开始

### 方式1：直接打开（推荐）

```bash
# 下载 模块1-直线往返相遇.html
# 双击在浏览器中打开
```

### 方式2：本地服务器

```bash
# 使用Python启动简单服务器
python3 -m http.server 8000

# 访问 http://localhost:8000
```

## 📖 使用说明

### 配置参数

- **出发模式**: 两端出发 / 同端出发
- **两地距离(S)**: 50-500米
- **甲速度**: 1-20 m/s
- **乙速度**: 1-20 m/s

### 观察重点

1. **实时动画区域**（上方）
   - 甲乙在同一直线上运动
   - 颜色区分：甲（红色）、乙（蓝色）
   - 实时显示位置和方向

2. **历史快照区域**（下方）
   - 每次相遇后的完整轨迹
   - 轨迹按折返次数自动下移
   - 方向箭头显示运动方向
   - 右侧标签显示相遇时刻

### 验证公式

- **两端出发**: (2n-1)S
  - 第1次: 1S
  - 第2次: 3S
  - 第3次: 5S
  - 第4次: 7S

- **同端出发**: 2nS
  - 第1次: 2S
  - 第2次: 4S
  - 第3次: 6S
  - 第4次: 8S

## 🛠️ 技术栈

- **HTML5** - 页面结构
- **Canvas API** - 动画绘制
- **Vanilla JavaScript** - 核心逻辑（零依赖）
- **LocalStorage** - 参数本地存储

## 📦 项目结构

```
.
├── 模块1-直线往返相遇.html    # 主文件（单文件运行）
└── README.md                   # 项目说明
```

## 🎨 设计系统

采用 **Notion风格** 设计系统：

```css
/* 颜色系统 */
--bg-primary: #F7F6F3;      /* 温暖米白 */
--bg-secondary: #FFFFFF;    /* 纯白卡片 */
--accent-brown: #C28B5D;    /* 棕色强调 */
--accent-red: #E03E3E;      /* 甲颜色 */
--accent-blue: #5E8AD2;     /* 乙颜色 */

/* 字体系统 */
--font-serif: 'Georgia';    /* 标题 */
--font-sans: 系统字体;       /* 正文 */
```

## 🚀 部署

### Cloudflare Pages

1. 推送代码到 GitHub
2. 在 Cloudflare Pages 连接仓库
3. 自动部署完成

### Vercel

```bash
npm i -g vercel
vercel --prod
```

## 📝 开发路线图

### v3.1 计划
- [ ] 添加预设题目系统（10+经典题型）
- [ ] 支持导出动画为GIF
- [ ] 添加慢动作回放功能

### v4.0 愿景
- [ ] 多物体追及（3-4个物体）
- [ ] 非同点出发的环形问题
- [ ] 复杂场景：走走停停+变速

## 📄 许可证

[MIT License](LICENSE)

## 🙏 致谢

- 设计灵感来自 [Notion](https://notion.so)
- 感谢 Claude Code 提供技术实现

## 📮 联系方式

- GitHub: [boing1002/linear-meeting-visualizer](https://github.com/boing1002/linear-meeting-visualizer)
- 问题反馈: [GitHub Issues](https://github.com/boing1002/linear-meeting-visualizer/issues)

---

**Made with ❤️ for math teachers and students**

**v3.0 - 模块1独立版本** | 2026-04
