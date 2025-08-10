# 🧭 Starter - 轻量级浏览器起始页

<!-- 语言切换导航 -->
<div align="center">
  <a href="#zh" style="margin: 0 8px; text-decoration: none;">中文</a> |
  <a href="#zh-tw" style="margin: 0 8px; text-decoration: none;">繁体中文</a> |
  <a href="#ja" style="margin: 0 8px; text-decoration: none;">日本語</a> |
  <a href="#ko" style="margin: 0 8px; text-decoration: none;">한국어</a> |
  <a href="#en" style="margin: 0 8px; text-decoration: none;">English</a> |
  <a href="#fr" style="margin: 0 8px; text-decoration: none;">Français</a> |
  <a href="#ru" style="margin: 0 8px; text-decoration: none;">Русский</a>
</div>


## <a id="zh"></a> 中文版本

Starter 是一个简洁、美观且高度可定制的浏览器起始页，专注于提供快速搜索体验和个性化内容展示。通过简单的配置，你可以将其打造成专属于自己的浏览器入口。


### ✨ 功能特点

- **多搜索引擎支持**：内置多种搜索引擎切换，支持保存个人偏好
- **个性化内容展示**：支持显示自定义文本、当前时间或随机一言
- **视觉定制**：可自定义背景图片、标题颜色等视觉元素
- **响应式设计**：完美适配桌面和移动设备
- **流畅动画**：添加了淡入、过渡等动画效果提升体验
- **本地存储**：自动保存用户偏好设置
- **防误操作**：禁止页面文本选择，避免误操作
- **精美字体**：采用小米 MiSans 字体，提供优秀的视觉体验


### 🚀 安装使用

1. **克隆项目**：
   ```bash
   git clone https://github.com/yourusername/starter-page.git
   cd starter-page
   ```

2. **准备资源**：
   - 将背景图片放入 `assets/img/` 目录
   - 将搜索引擎图标放入 `assets/img/icons/` 目录
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
├── assets/           # 资源目录
│   ├── css/          # 样式表目录
│   │   └── style.css # 主要样式表文件
│   ├── js/           # 脚本目录
│   │   └── script.js # 主要交互脚本文件
│   ├── font/         # 字体文件目录（包含MiSans）
│   └── img/          # 图片资源目录
│       ├── icons/    # 搜索引擎图标目录
│       └── bg.jpg    # 背景图片示例
├── index.html        # 主页面
├── config.json       # 配置文件
└── README.md         # 说明文档

### 🙏 鸣谢

本项目使用了以下优秀的开源资源：

- [Tailwind CSS](https://tailwindcss.com/) - 实用优先的CSS框架
- [Font Awesome](https://fontawesome.com/) - 图标库
- [Hitokoto API](https://hitokoto.cn/) - 提供一言内容
- [MiSans](https://hyperos.mi.com/font/zh/) - 小米官方字体


### 📝 许可证

本项目采用 [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可证开源。


## <a id="zh-tw"></a> 繁體中文版本

Starter 是一個簡潔、美觀且高度可定制的瀏覽器起始頁，專注於提供快速搜索體驗和個性化內容展示。通過簡單的配置，你可以將其打造成專屬於自己的瀏覽器入口。


### ✨ 功能特點

- **多搜索引擎支持**：內置多種搜索引擎切換，支持保存個人偏好
- **個性化內容展示**：支持顯示自定義文本、當前時間或隨機一言
- **視覺定制**：可自定義背景圖片、標題顏色等視覺元素
- **響應式設計**：完美適配桌面和移動設備
- **流暢動畫**：添加了淡入、過渡等動畫效果提升體驗
- **本地存儲**：自動保存用戶偏好設置
- **防誤操作**：禁止頁面文本選擇，避免誤操作
- **精美字體**：採用小米 MiSans 字體，提供優秀的視覺體驗


### 🚀 安裝使用

1. **克隆項目**：
   ```bash
   git clone https://github.com/yourusername/starter-page.git
   cd starter-page
   ```

2. **準備資源**：
   - 將背景圖片放入 `assets/img/` 目錄
   - 將搜索引擎圖標放入 `assets/img/icons/` 目錄
   - MiSans 字體已配置，如需更新可替換 `assets/font/` 目錄下的字體文件

3. **配置頁面**：
   復制 `config.example.json` 為 `config.json`，根據需求修改配置（詳見配置說明）

4. **啟動使用**：
   直接在瀏覽器中打開 `index.html` 文件，或部署到web服務器


### ⚙️ 配置說明

`config.json` 是頁面的核心配置文件，主要包含以下配置項：

| 配置項 | 說明 | 示例值 |
|--------|------|--------|
| `mainTitle` | 主標題內容，支持特殊值 `--time--`（顯示時間）或 `--hitokoto--`（顯示一言） | `"快速搜索"` |
| `subTitle` | 副標題內容，支持同上特殊值 | `"探索互聯網的起點"` |
| `mainTitleColor` | 主標題顏色 | `"#ffffff"` |
| `subTitleColor` | 副標題顏色 | `"#e2e8f0"` |
| `backgroundImage` | 背景圖片路徑（留空則使用默認背景色） | `"assets/img/bg.jpg"` |
| `defaultSearchEngine` | 默認搜索引擎ID | `"baidu"` |
| `searchEngines` | 搜索引擎配置數組 | 詳見下方示例 |

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

### 🎨 自定義樣式

除了基礎配置外，你還可以通過修改以下文件進一步定制樣式：

- `assets/css/style.css` - 主要樣式表文件
- `assets/js/script.js` - 交互腳本文件
- 修改 `@font-face` 配置更換自定義字體
- 調整 `tailwind.config` 中的顏色配置修改主題色
- 修改動畫關鍵幀調整過渡效果
- 調整背景模糊、透明度等視覺效果


### 📄 項目結構starter-page/
├── assets/           # 資源目錄
│   ├── css/          # 樣式表目錄
│   │   └── style.css # 主要樣式表文件
│   ├── js/           # 腳本目錄
│   │   └── script.js # 主要交互腳本文件
│   ├── font/         # 字體文件目錄（包含MiSans）
│   └── img/          # 圖片資源目錄
│       ├── icons/    # 搜索引擎圖標目錄
│       └── bg.jpg    # 背景圖片示例
├── index.html        # 主頁面
├── config.json       # 配置文件
└── README.md         # 說明文檔

### 🙏 鳴謝

本項目使用了以下優秀的開源資源：

- [Tailwind CSS](https://tailwindcss.com/) - 實用優先的CSS框架
- [Font Awesome](https://fontawesome.com/) - 圖標庫
- [Hitokoto API](https://hitokoto.cn/) - 提供一言內容
- [MiSans](https://hyperos.mi.com/font/zh/) - 小米官方字體


### 📝 許可證

本項目採用 [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 許可證開源。


## <a id="ja"></a> 日本語バージョン

Starterは、シンプルで美しく、高度にカスタマイズ可能なブラウザのスタートページです。クイック検索機能と个性化されたコンテンツ表示に特化しており、簡単な設定で自分だけのブラウザ入口に変えることができます。


### ✨ 主な機能

- **複数検索エンジン支持**：複数の検索エンジンを切り替え可能で、個人の設定を保存できます
- **个性化コンテンツ表示**：カスタムテキスト、現在時間、またはランダムな一言を表示できます
- **視覚カスタマイズ**：背景画像、タイトル色などの視覚要素をカスタマイズ可能
- **レスポンシブデザイン**：デスクトップとモバイルデバイスに最適化
- **スムーズなアニメーション**：フェードイン、トランジションなどのアニメーション効果を追加
- **ローカルストレージ**：ユーザーの設定を自動的に保存
- **誤操作防止**：ページテキストの選択を禁止し、誤操作を防ぐ
- **美しいフォント**：小米のMiSansフォントを採用し、優れた視覚体験を提供


### 🚀 インストールと使用

1. **プロジェクトをクローン**：
   ```bash
   git clone https://github.com/yourusername/starter-page.git
   cd starter-page
   ```

2. **リソースの準備**：
   - 背景画像を `assets/img/` ディレクトリに配置
   - 検索エンジンのアイコンを `assets/img/icons/` ディレクトリに配置
   - MiSansフォントはすでに設定されています。更新する場合は `assets/font/` ディレクトリのフォントファイルを置き換えてください

3. **ページの設定**：
   `config.example.json` を `config.json` としてコピーし、ニーズに応じて設定を変更します（設定の詳細は設定説明を参照）

4. **使用開始**：
   ブラウザで `index.html` ファイルを直接開くか、webサーバーにデプロイしてください


### ⚙️ 設定の説明

`config.json` はページの核心設定ファイルで、主に以下の設定項目が含まれています：

| 設定項目 | 説明 | 例 |
|--------|------|--------|
| `mainTitle` | メインタイトルの内容。特殊値 `--time--`（時間表示）または `--hitokoto--`（一言表示）をサポート | `"クイック検索"` |
| `subTitle` | サブタイトルの内容。上記の特殊値をサポート | `"インターネット探索の起点"` |
| `mainTitleColor` | メインタイトルの色 | `"#ffffff"` |
| `subTitleColor` | サブタイトルの色 | `"#e2e8f0"` |
| `backgroundImage` | 背景画像のパス（空の場合はデフォルトの背景色を使用） | `"assets/img/bg.jpg"` |
| `defaultSearchEngine` | デフォルトの検索エンジンID | `"baidu"` |
| `searchEngines` | 検索エンジンの設定配列 | 以下の例を参照 |

#### 検索エンジン設定の例"searchEngines": [
  {
    "id": "baidu",
    "name": "百度",
    "icon": "assets/img/icons/baidu.png",
    "url": "https://www.baidu.com/s?wd=%search"
  },
  {
    "id": "google",
    "name": "Google",
    "icon": "assets/img/icons/google.png",
    "url": "https://www.google.com/search?q=%search"
  }
]

### 🎨 スタイルのカスタマイズ

基本設定に加えて、以下のファイルを変更することでさらにスタイルをカスタマイズできます：

- `assets/css/style.css` - 主なスタイルシートファイル
- `assets/js/script.js` - インタラクションスクリプトファイル
- `@font-face` 設定を変更してカスタムフォントに置き換える
- `tailwind.config` の色設定を調整してテーマカラーを変更
- アニメーションキーフレームを変更してトランジション効果を調整
- 背景のぼかし、透明度などの視覚効果を調整


### 📄 プロジェクト構造starter-page/
├── assets/           # リソースディレクトリ
│   ├── css/          # スタイルシートディレクトリ
│   │   └── style.css # 主なスタイルシートファイル
│   ├── js/           # スクリプトディレクトリ
│   │   └── script.js # 主なインタラクションスクリプトファイル
│   ├── font/         # フォントファイルディレクトリ（MiSansを含む）
│   └── img/          # 画像リソースディレクトリ
│       ├── icons/    # 検索エンジンアイコンディレクトリ
│       └── bg.jpg    # 背景画像の例
├── index.html        # メインページ
├── config.json       # 設定ファイル
└── README.md         # 説明ドキュメント

### 🙏 謝辞

本プロジェクトは以下の優れたオープンソースリソースを使用しています：

- [Tailwind CSS](https://tailwindcss.com/) - ユーティリティファーストのCSSフレームワーク
- [Font Awesome](https://fontawesome.com/) - アイコンライブラリ
- [Hitokoto API](https://hitokoto.cn/) - 一言コンテンツを提供
- [MiSans](https://hyperos.mi.com/font/zh/) - 小米公式フォント


### 📝 ライセンス

本プロジェクトは [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) ライセンスに基づいてオープンソースとして公開されています。


## <a id="ko"></a> 한국어 버전

Starter는 간결하고美观하며高度로 사용자 정의가 가능한 브라우저 시작 페이지입니다. 빠른 검색 경험과 개인화된 콘텐츠 표시에 중점을 두고 있으며, 간단한 설정을 통해 자신만의 브라우저 진입점으로 꾸밀 수 있습니다.


### ✨ 주요 기능

- **다중 검색 엔진 지원**: 다양한 검색 엔진 간 전환이 가능하며, 개인 선호 설정을 저장할 수 있습니다
- **개인화 콘텐츠 표시**: 사용자 정의 텍스트, 현재 시간 또는 랜덤 한마디 표시를 지원합니다
- **시각적 사용자 정의**: 배경 이미지, 제목 색상 등 시각적 요소를 사용자 정의할 수 있습니다
- **반응형 디자인**: 데스크톱과 모바일 장치에 완벽히 적응합니다
- **부드러운 애니메이션**: 페이드 인, 전환 등 애니메이션 효과를 추가하여 사용体验를 향상시킵니다
- **로컬 저장**: 사용자 선호 설정을 자동으로 저장합니다
- **오작동 방지**: 페이지 텍스트 선택을 금지하여 오작동을 방지합니다
- **고급 글꼴**: 샤오미 MiSans 글꼴을 채택하여 우수한 시각体验를 제공합니다


### 🚀 설치 및 사용

1. **프로젝트 클론**:
   ```bash
   git clone https://github.com/yourusername/starter-page.git
   cd starter-page
   ```

2. **리소스 준비**:
   - 배경 이미지를 `assets/img/` 디렉토리에 넣습니다
   - 검색 엔진 아이콘을 `assets/img/icons/` 디렉토리에 넣습니다
   - MiSans 글꼴은 이미 구성되어 있습니다. 업데이트하려면 `assets/font/` 디렉토리의 글꼴 파일을 교체하십시오

3. **페이지 구성**:
   `config.example.json`을 `config.json`으로 복사하고 요구에 따라 구성을 수정합니다(구성 설명 참조)

4. **사용 시작**:
   브라우저에서 `index.html` 파일을 직접 열거나 웹 서버에 배포하십시오


### ⚙️ 구성 설명

`config.json`은 페이지의 핵심 구성 파일으로, 주로 다음 구성 항목을 포함합니다:

| 구성 항목 | 설명 | 예시 값 |
|--------|------|--------|
| `mainTitle` | 주 제목 내용, 특수 값 `--time--`(시간 표시) 또는 `--hitokoto--`(한마디 표시) 지원 | `"빠른 검색"` |
| `subTitle` | 부 제목 내용, 위의 특수 값 지원 | `"인터넷 탐험의 시작점"` |
| `mainTitleColor` | 주 제목 색상 | `"#ffffff"` |
| `subTitleColor` | 부 제목 색상 | `"#e2e8f0"` |
| `backgroundImage` | 배경 이미지 경로(비어 있으면 기본 배경색 사용) | `"assets/img/bg.jpg"` |
| `defaultSearchEngine` | 기본 검색 엔진 ID | `"baidu"` |
| `searchEngines` | 검색 엔진 구성 배열 | 아래 예시 참조 |

#### 검색 엔진 구성 예시"searchEngines": [
  {
    "id": "baidu",
    "name": "바이두",
    "icon": "assets/img/icons/baidu.png",
    "url": "https://www.baidu.com/s?wd=%search"
  },
  {
    "id": "google",
    "name": "구글",
    "icon": "assets/img/icons/google.png",
    "url": "https://www.google.com/search?q=%search"
  }
]

### 🎨 스타일 사용자 정의

기본 구성 외에도 다음 파일을 수정하여 스타일을 추가로 사용자 정의할 수 있습니다:

- `assets/css/style.css` - 주요 스타일시트 파일
- `assets/js/script.js` - 상호작용 스크립트 파일
- `@font-face` 구성을 수정하여 사용자 정의 글꼴로 바꿉니다
- `tailwind.config`의 색상 구성을 조정하여 테마 색상을 변경합니다
- 애니메이션 키프레임을 수정하여 전환 효과를 조정합니다
- 배경 블러, 투명도 등 시각적 효과를 조정합니다


### 📄 프로젝트 구조starter-page/
├── assets/           # 리소스 디렉토리
│   ├── css/          # 스타일시트 디렉토리
│   │   └── style.css # 주요 스타일시트 파일
│   ├── js/           # 스크립트 디렉토리
│   │   └── script.js # 주요 상호작용 스크립트 파일
│   ├── font/         # 글꼴 파일 디렉토리(MiSans 포함)
│   └── img/          # 이미지 리소스 디렉토리
│       ├── icons/    # 검색 엔진 아이콘 디렉토리
│       └── bg.jpg    # 배경 이미지 예시
├── index.html        # 메인 페이지
├── config.json       # 구성 파일
└── README.md         # 설명 문서

### 🙏 감사의 말

본 프로젝트는 다음 우수한 오픈 소스 리소스를 사용하였습니다:

- [Tailwind CSS](https://tailwindcss.com/) - 유틸리티 우선 CSS 프레임워크
- [Font Awesome](https://fontawesome.com/) - 아이콘 라이브러리
- [Hitokoto API](https://hitokoto.cn/) - 한마디 콘텐츠 제공
- [MiSans](https://hyperos.mi.com/font/zh/) - 샤오미 공식 글꼴


### 📝 라이센스

본 프로젝트는 [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 라이센스를 채택하여 오픈 소스로 공개합니다.


## <a id="en"></a> English Version

Starter is a clean, beautiful, and highly customizable browser start page, focused on providing a quick search experience and personalized content display. With simple configurations, you can turn it into your own unique browser entrance.


### ✨ Features

- **Multiple search engines support**: Built-in switch between various search engines with personal preference saving
- **Personalized content display**: Supports custom text, current time, or random quotes
- **Visual customization**: Customizable background images, title colors and other visual elements
- **Responsive design**: Perfectly adapts to desktop and mobile devices
- **Smooth animations**: Added fade-in, transition and other animation effects to enhance experience
- **Local storage**: Automatically saves user preferences
- **Misoperation prevention**: Disables page text selection to avoid mistakes
- **Premium font**: Uses Xiaomi MiSans font for excellent visual experience


### 🚀 Installation and Usage

1. **Clone the project**:
   ```bash
   git clone https://github.com/yourusername/starter-page.git
   cd starter-page
   ```

2. **Prepare resources**:
   - Place background images in the `assets/img/` directory
   - Place search engine icons in the `assets/img/icons/` directory
   - MiSans font is pre-configured; to update, replace files in the `assets/font/` directory

3. **Configure the page**:
   Copy `config.example.json` to `config.json` and modify according to your needs (see configuration instructions for details)

4. **Start using**:
   Open the `index.html` file directly in your browser or deploy to a web server


### ⚙️ Configuration Instructions

`config.json` is the core configuration file for the page, containing the following main configuration items:

| Configuration Item | Description | Example Value |
|--------|------|--------|
| `mainTitle` | Main title content, supports special values `--time--` (show time) or `--hitokoto--` (show quote) | `"Quick Search"` |
| `subTitle` | Subtitle content, supports the same special values as above | `"Starting point for internet exploration"` |
| `mainTitleColor` | Main title color | `"#ffffff"` |
| `subTitleColor` | Subtitle color | `"#e2e8f0"` |
| `backgroundImage` | Background image path (leave empty to use default background color) | `"assets/img/bg.jpg"` |
| `defaultSearchEngine` | Default search engine ID | `"baidu"` |
| `searchEngines` | Search engine configuration array | See example below |

#### Search Engine Configuration Example"searchEngines": [
  {
    "id": "baidu",
    "name": "Baidu",
    "icon": "assets/img/icons/baidu.png",
    "url": "https://www.baidu.com/s?wd=%search"
  },
  {
    "id": "google",
    "name": "Google",
    "icon": "assets/img/icons/google.png",
    "url": "https://www.google.com/search?q=%search"
  }
]

### 🎨 Customizing Styles

In addition to basic configurations, you can further customize styles by modifying the following files:

- `assets/css/style.css` - Main stylesheet file
- `assets/js/script.js` - Interaction script file
- Modify `@font-face` configuration to change to custom fonts
- Adjust color configurations in `tailwind.config` to modify theme colors
- Modify animation keyframes to adjust transition effects
- Adjust background blur, transparency and other visual effects


### 📄 Project Structurestarter-page/
├── assets/           # Resource directory
│   ├── css/          # Stylesheet directory
│   │   └── style.css # Main stylesheet file
│   ├── js/           # Script directory
│   │   └── script.js # Main interaction script file
│   ├── font/         # Font files directory (including MiSans)
│   └── img/          # Image resources directory
│       ├── icons/    # Search engine icons directory
│       └── bg.jpg    # Background image example
├── index.html        # Main page
├── config.json       # Configuration file
└── README.md         # Documentation

### 🙏 Acknowledgments

This project uses the following excellent open-source resources:

- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Font Awesome](https://fontawesome.com/) - Icon library
- [Hitokoto API](https://hitokoto.cn/) - Provides quote content
- [MiSans](https://hyperos.mi.com/font/zh/) - Xiaomi official font


### 📝 License

This project is open-sourced under the [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.


## <a id="fr"></a> Version Française

Starter est une page de démarrage de navigateur propre, belle et hautement personnalisable, axée sur la fourniture d'une expérience de recherche rapide et d'un affichage de contenu personnalisé. Grâce à de simples configurations, vous pouvez en faire une entrée de navigateur unique.


### ✨ Fonctionnalités

- **Support de plusieurs moteurs de recherche** : Commutation intégrée entre divers moteurs de recherche avec sauvegarde des préférences personnelles
- **Affichage de contenu personnalisé** : Prend en charge le texte personnalisé, l'heure actuelle ou les citations aléatoires
- **Personnalisation visuelle** : Images de fond, couleurs de titre et autres éléments visuels personnalisables
- **Design responsive** : S'adapte parfaitement aux ordinateurs de bureau et aux appareils mobiles
- **Animations fluides** : Ajout d'effets d'animation comme le fondu, la transition pour améliorer l'expérience
- **Stockage local** : Enregistre automatiquement les préférences de l'utilisateur
- **Prévention des erreurs** : Désactive la sélection de texte pour éviter les erreurs
- **Police de qualité** : Utilise la police MiSans de Xiaomi pour une excellente expérience visuelle


### 🚀 Installation et utilisation

1. **Cloner le projet** :
   ```bash
   git clone https://github.com/yourusername/starter-page.git
   cd starter-page
   ```

2. **Préparer les ressources** :
   - Placez les images de fond dans le dossier `assets/img/`
   - Placez les icônes des moteurs de recherche dans le dossier `assets/img/icons/`
   - La police MiSans est préconfigurée ; pour la mettre à jour, remplacez les fichiers dans le dossier `assets/font/`

3. **Configurer la page** :
   Copiez `config.example.json` en `config.json` et modifiez-le selon vos besoins (voir les instructions de configuration pour plus de détails)

4. **Commencer à utiliser** :
   Ouvrez le fichier `index.html` directement dans votre navigateur ou déployez-le sur un serveur web


### ⚙️ Instructions de configuration

`config.json` est le fichier de configuration principal de la page, contenant les éléments de configuration suivants :

| Élément de configuration | Description | Valeur exemple |
|--------|------|--------|
| `mainTitle` | Contenu du titre principal, prend en charge les valeurs spéciales `--time--` (afficher l'heure) ou `--hitokoto--` (afficher une citation) | `"Recherche rapide"` |
| `subTitle` | Contenu du sous-titre, prend en charge les mêmes valeurs spéciales que ci-dessus | `"Point de départ pour l'exploration internet"` |
| `mainTitleColor` | Couleur du titre principal | `"#ffffff"` |
| `subTitleColor` | Couleur du sous-titre | `"#e2e8f0"` |
| `backgroundImage` | Chemin de l'image de fond (laissez vide pour utiliser la couleur de fond par défaut) | `"assets/img/bg.jpg"` |
| `defaultSearchEngine` | ID du moteur de recherche par défaut | `"baidu"` |
| `searchEngines` | Tableau de configuration des moteurs de recherche | Voir l'exemple ci-dessous |

#### Exemple de configuration de moteur de recherche"searchEngines": [
  {
    "id": "baidu",
    "name": "Baidu",
    "icon": "assets/img/icons/baidu.png",
    "url": "https://www.baidu.com/s?wd=%search"
  },
  {
    "id": "google",
    "name": "Google",
    "icon": "assets/img/icons/google.png",
    "url": "https://www.google.com/search?q=%search"
  }
]

### 🎨 Personnalisation des styles

En plus des configurations de base, vous pouvez personnaliser davantage les styles en modifiant les fichiers suivants :

- `assets/css/style.css` - Fichier de feuille de style principal
- `assets/js/script.js` - Fichier de script d'interaction
- Modifiez la configuration `@font-face` pour changer de police
- Ajustez les configurations de couleur dans `tailwind.config` pour modifier les couleurs du thème
- Modifiez les keyframes d'animation pour ajuster les effets de transition
- Ajustez le flou d'arrière-plan, la transparence et autres effets visuels


### 📄 Structure du projetstarter-page/
├── assets/           # Dossier des ressources
│   ├── css/          # Dossier de feuilles de style
│   │   └── style.css # Fichier de feuille de style principal
│   ├── js/           # Dossier de scripts
│   │   └── script.js # Fichier de script d'interaction principal
│   ├── font/         # Dossier de fichiers de police (y compris MiSans)
│   └── img/          # Dossier de ressources image
│       ├── icons/    # Dossier d'icônes de moteurs de recherche
│       └── bg.jpg    # Exemple d'image de fond
├── index.html        # Page principale
├── config.json       # Fichier de configuration
└── README.md         # Documentation

### 🙏 Remerciements

Ce projet utilise les excellentes ressources open-source suivantes :

- [Tailwind CSS](https://tailwindcss.com/) - Framework CSS utilitaire
- [Font Awesome](https://fontawesome.com/) - Bibliothèque d'icônes
- [Hitokoto API](https://hitokoto.cn/) - Fournit du contenu de citations
- [MiSans](https://hyperos.mi.com/font/zh/) - Police officielle de Xiaomi


### 📝 Licence

Ce projet est open-source sous licence [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).


## <a id="ru"></a> Русская версия

Starter — это чистая, красивая и сильно настраиваемая стартовая страница браузера, ориентированная на быстрое выполнение поисковых запросов и отображение персонализированного контента. С помощью простых настроек вы можете превратить её в уникальную точку входа в интернет.


### ✨ Основные функции

- **Поддержка нескольких поисковых систем**: Встроенный переключатель между различными поисковыми системами с сохранением личных предпочтений
- **Показ персонализированного контента**: Поддержка пользовательского текста, текущего времени или случайных цитат
- **Визуальная настройка**: Настраиваемые фоновые изображения, цвета заголовков и другие визуальные элементы
- **Адаптивный дизайн**: Идеально подходит для настольных компьютеров и мобильных устройств
- **Плавные анимации**: Добавлены эффекты появления, перехода и других анимаций для улучшения пользовательского опыта
- **Локальное хранение**: Автоматическое сохранение предпочтений пользователя
- **Предотвращение ошибок**: Отключение выделения текста на странице для избежания ошибок操作
- **Премиум-шрифт**: Использует шрифт MiSans от Xiaomi для отличного визуального восприятия


### 🚀 Установка и использование

1. **Клонирование проекта**:
   ```bash
   git clone https://github.com/yourusername/starter-page.git
   cd starter-page
   ```

2. **Подготовка ресурсов**:
   - Поместите фоновые изображения в каталог `assets/img/`
   - поместите иконки поисковых систем в каталог `assets/img/icons/`
   - Шрифт MiSans уже настроен; для обновления замените файлы в каталоге `assets/font/`

3. **Настройка страницы**:
   Скопируйте `config.example.json` в `config.json` и измените в соответствии с вашими потребностями (см. детали в инструкции по настройке)

4. **Начало использования**:
   Откройте файл `index.html` напрямую в браузере или разверните на веб-сервере


### ⚙️ Инструкции по настройке

`config.json` — основной конфигурационный файл страницы, содержащий следующие основные параметры:

| Параметр конфигурации | Описание | Пример значения |
|--------|------|--------|
| `mainTitle` | Содержимое основного заголовка, поддерживает специальные значения `--time--` (показ времени) или `--hitokoto--` (показ цитаты) | `"Быстрый поиск"` |
| `subTitle` | Содержимое подзаголовка, поддерживает те же специальные значения | `"Точка отправления для интернет-исследований"` |
| `mainTitleColor` | Цвет основного заголовка | `"#ffffff"` |
| `subTitleColor` | Цвет подзаголовка | `"#e2e8f0"` |
| `backgroundImage` | Путь к фоновому изображению (оставьте пустым, чтобы использовать цвет фона по умолчанию) | `"assets/img/bg.jpg"` |
| `defaultSearchEngine` | ID поисковой системы по умолчанию | `"baidu"` |
| `searchEngines` | Массив конфигураций поисковых систем | См. пример ниже |

#### Пример конфигурации поисковой системы"searchEngines": [
  {
    "id": "baidu",
    "name": "Байду",
    "icon": "assets/img/icons/baidu.png",
    "url": "https://www.baidu.com/s?wd=%search"
  },
  {
    "id": "google",
    "name": "Гугл",
    "icon": "assets/img/icons/google.png",
    "url": "https://www.google.com/search?q=%search"
  }
]

### 🎨 Настройка стилей

Помимо базовых настроек, вы можете дополнительно настроить стили, изменив следующие файлы:

- `assets/css/style.css` — Основной файл стилей
- `assets/js/script.js` — Файл интерактивных скриптов
- Измените конфигурацию `@font-face`, чтобы сменить шрифт
- Настройте цветовые параметры в `tailwind.config`, чтобы изменить цвета темы
- Измените ключевые кадры анимации, чтобы настроить эффекты перехода
- Регулируйте размытие фона, прозрачность и другие визуальные эффекты


### 📄 Структура проектаstarter-page/
├── assets/           # Каталог ресурсов
│   ├── css/          # Каталог стилей
│   │   └── style.css # Основной файл стилей
│   ├── js/           # Каталог скриптов
│   │   └── script.js # Основной файл интерактивных скриптов
│   ├── font/         # Каталог шрифтов (включая MiSans)
│   └── img/          # Каталог изображений
│       ├── icons/    # Каталог иконок поисковых систем
│       └── bg.jpg    # Пример фонового изображения
├── index.html        # Основная страница
├── config.json       # Конфигурационный файл
└── README.md         # Документация

### 🙏 Благодарности

Этот проект использует следующие отличные открытые ресурсы:

- [Tailwind CSS](https://tailwindcss.com/) — Утилитарный CSS-фреймворк
- [Font Awesome](https://fontawesome.com/) — Библиотека иконок
- [Hitokoto API](https://hitokoto.cn/) — Предоставляет содержимое цитат
- [MiSans](https://hyperos.mi.com/font/zh/) — Официальный шрифт Xiaomi


### 📝 Лицензия

Этот проект распространяется под лицензией [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
```
