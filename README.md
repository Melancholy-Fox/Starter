# 🧭 Starter - 轻量级浏览器起始页

Starter 是一个简洁、美观且高度可定制的浏览器起始页，专注于提供快速搜索体验和个性化内容展示。通过简单的配置，你可以将其打造成专属于自己的浏览器入口。


### ✨ 功能特点

- **多搜索引擎支持**：内置多种搜索引擎切换，支持保存个人偏好
- **个性化内容展示**：支持显示自定义文本、当前时间或随机一言
- **视觉定制**：可自定义背景图片、标题颜色等视觉元素
- **响应式设计**：完美适配桌面和移动设备
- **流畅动画**：添加了淡入、过渡等动画效果提升体验
- **本地存储**：自动保存用户偏好设置
- **精美字体**：采用小米 MiSans 字体，提供优秀的视觉体验


### 🚀 安装使用

1. **克隆项目**：
   ```bash
   git clone https://github.com/yourusername/starter-page.git
   cd starter-page
   ```

2. **准备资源**：
   - 将图片放入 `assets/img/` 目录
   - MiSans 字体已配置，如需更新可替换 `assets/font/` 目录下的字体文件

3. **配置页面**：
   复制 `config.example.json` 为 `config.json`，根据需求修改配置（详见配置说明）

4. **启动使用**：
   直接在浏览器中打开 `index.html` 文件，或部署到web服务器


### ⚙️ 配置说明

`config.json` 是页面的核心配置文件，主要包含以下配置项：

| 配置项 | 说明 | 示例值 |
|--------|------|--------|
| `mainTitle` | 主标题内容，支持特殊值 `--time--`（显示时间）或 `--hitokoto--`（显示一言） | `"快速搜索"` |
| `subTitle` | 副标题内容，支持同上特殊值 | `"探索互联网的起点"` |
| `mainTitleColor` | 主标题颜色 | `"#ffffff"` |
| `subTitleColor` | 副标题颜色 | `"#e2e8f0"` |
| `backgroundImage` | 背景图片路径（留空则使用默认背景色） | `"assets/img/bg.jpg"` |
| `defaultSearchEngine` | 默认搜索引擎ID | `"baidu"` |
| `searchEngines` | 搜索引擎配置数组 | 详见下方示例 |

#### 搜索引擎配置示例"searchEngines": [
  {
    "id": "baidu",
    "name": "百度",
    "icon": "assets/img/icons/baidu.png",
    "url": "https://www.baidu.com/s?wd=%search"
  },
  {
    "id": "google",
    "name": "谷歌",
    "icon": "assets/img/icons/google.png",
    "url": "https://www.google.com/search?q=%search"
  }
]

### 🎨 自定义样式

除了基础配置外，你还可以通过修改以下文件进一步定制样式：

- `assets/css/style.css` - 主要样式表文件
- `assets/js/script.js` - 交互脚本文件
- 修改 `@font-face` 配置更换自定义字体
- 调整 `tailwind.config` 中的颜色配置修改主题色
- 修改动画关键帧调整过渡效果
- 调整背景模糊、透明度等视觉效果


### 📄 项目结构starter-page/
├── assets/                       # 资源目录
│   ├── font/                     # 字体文件目录
│   │   └── Misans-Regular.ttf    # MiSans Font
│   └── img/                      # 图片资源目录
│       ├── icons/                # 搜索引擎图标目录
│       └── bg.jpg                # 背景图片示例
├── index.html                    # 主页面
├── config.json                   # 配置文件
└── README.md                     # 说明文档

### 🙏 鸣谢

本项目使用了以下优秀的开源资源：

- [Tailwind CSS](https://tailwindcss.com/) - 实用优先的CSS框架
- [Font Awesome](https://fontawesome.com/) - 图标库
- [Hitokoto API](https://hitokoto.cn/) - 提供一言内容
- [MiSans](https://hyperos.mi.com/font/zh/) - MiSans字体


### 📝 许可证

本项目采用 [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可证开源。
