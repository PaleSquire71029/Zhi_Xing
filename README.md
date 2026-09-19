# 🧭 知行导航 (Zhixing Hub)

> **极简高效网址聚合与效率中枢 —— 探索全网优质资源，一触即达。**

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML-5-orange.svg)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-yellow.svg)

知行导航是一个单文件 HTML 应用，无需后端服务器，开箱即用。它聚合了全网高质量的 AI、开发者、设计、学习、生活等各领域网址，并提供丰富的纯本地计算工具箱与私人书签管理功能，旨在打造优雅、高效的个人互联网探索与效率导航站。

![Zhixing Hub Banner](https://via.placeholder.com/1200x600/08090C/B09056?text=Zhixing+Hub+%E7%9F%A5%E8%A1%8C%E5%AF%BC%E8%88%AA)


---

## ✨ 核心特性

- 🎨 **高质感深色 UI**：采用暗金配色、毛玻璃（Glassmorphism）材质、动态粒子背景与平滑的入场动画，追求极致的视觉与交互体验。
- 🔍 **全域智能搜索**：
  - 支持一键切换 Google、Bing、Bilibili、GitHub 四大搜索引擎。
  - 内置站内搜索引擎，支持中文拼音全拼、首字母极速检索（无需回车，实时弹出下拉建议）。
  - 支持 `Ctrl/Cmd + K` 快捷键聚焦搜索。
- 🗂️ **精选网址大全**：内置 8 大类超 90 个精选优质站点，支持分类过滤、网格/列表视图切换，以及热门站点一键“钉选”至顶部快捷栏。
- 🛠️ **极客工具箱**：无需安装，纯前端本地计算，保护数据隐私。
  - 强密码生成器（一键生成高强度随机密码并自动复制）。
  - 字数统计与大小写格式化（实时计算字符、单词、行数）。
  - Base64 / URL 编解码器。
- ⭐ **私人专属书签**：支持添加、删除自定义网址。数据通过 `localStorage` 保存在本地浏览器，支持配置的 JSON 导出与导入，方便备份和跨设备迁移。
- 📱 **深度移动端适配**：响应式布局，针对手机屏幕对搜索框、选项卡和网格卡片进行了防截断优化，触屏体验顺滑。

---

## 🛠️ 技术栈

- **前端框架**：原生 HTML5 + Vanilla JavaScript（无复杂构建步骤）
- **样式框架**：Tailwind CSS (CDN JIT 模式)
- **图标库**：Font Awesome 6
- **字体**：Plus Jakarta Sans (英文/数字) + Noto Serif SC (中文)
- **拼音支持**：pinyin-pro（异步动态加载，失败自动降级为纯文本匹配）

---

## 🚀 快速开始

### 方式一：本地直接运行（推荐）

1. **下载或克隆本仓库**：
   ```bash
   git clone https://github.com/PaleSquire71029/zhixing-hub.git
   ```
2. **直接打开**：双击 `index.html` 文件，使用现代浏览器（Chrome、Edge、Safari、Firefox）打开即可。
   
   > 💡 **提示**：由于使用了 CDN 加速服务，首次打开需要保持网络畅通。不建议在本地文件管理器（如 MT 管理器）的内置浏览器中打开，可能会因缺少网络权限而导致样式丢失。

### 方式二：部署到静态托管平台（最佳体验）

您可以将该项目一键部署到以下平台，获得极佳的在线访问速度：

- [Vercel](https://vercel.com/)
- [Netlify](https://www.netlify.com/)
- [GitHub Pages](https://pages.github.com/)
- [Gitee Pages](https://gitee.com/help/articles/4136)

---

## 📁 项目结构

```text
zhixing-hub/
├── index.html       # 单文件应用（包含所有 HTML、CSS、JS）
└── README.md        # 项目说明文档
```

---

## 📝 自定义与扩展

如果您想添加或修改内置的网址，只需在 `index.html` 中找到 `defaultWebsites` 数组，按以下格式添加即可：

```javascript
{ 
  id: 'custom_1', 
  name: "网站名称", 
  url: "https://example.com", 
  icon: "fa-solid fa-globe", 
  color: "text-blue-400", 
  bg: "bg-blue-500/10", 
  desc: "网站简短描述", 
  category: "tools", // 对应分类：ai, dev, tools, design, entertainment, game, learning, life
  hot: true 
}
```

---

## 🤝 反馈与交流

如果您有任何建议、Bug 反馈或想交流技术，欢迎通过以下方式联系我：

- **邮箱**：palesquire71029@qq.com
- **GitHub**：[@PaleSquire71029](https://github.com/PaleSquire71029)
- **Bilibili**：[@逐浪的红叶](https://space.bilibili.com/1474060600)
- **YouTube**：[@逐浪的红叶](https://youtube.com/@ccc-lc3ct)

---

## 📄 开源协议

本项目采用 [MIT License](LICENSE) 协议开源。您可以自由使用、修改和分发，但请保留原作者信息。