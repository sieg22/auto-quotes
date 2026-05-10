# Auto Quotes · 好句摘抄生成器

**中文** | [English](#english)

一个为手帐爱好者和练字爱好者设计的好句摘抄工具。支持中、英、日、法、韩五种语言，随机抓取文学名著、哲学思想、诗歌、歌词中的佳句，配合字体切换功能，方便对照练字。

🔗 **在线访问：** https://sieg22.github.io/auto-quotes/


---

## 功能特性

- **五语言内容**：中文 / English / 日本語 / Français / 한국어
- **两种长度**：长段摘抄/ 短金句
- **多内容分类**：文学小说 · 哲学思想 · 诗词 · 更多
- **多字体切换**：支持本地自定义字体，切换字体对照练习
- **私藏收藏**：一键收藏喜欢的句子，双击收藏条目可还原到主窗口
- **日夜模式**：护眼暗色主题
- **界面双语**：右上角 中 / En 切换界面语言
- **随机色调**：每次翻页自动切换暖色调配色
- **零依赖**：纯 HTML + CSS + JavaScript，无需安装，无需服务器

---

## 数据来源

- [Wikiquote](https://www.wikiquote.org)（zh / en / ja / fr / ko，MediaWiki API，CORS 开放）
- [Hitokoto 一言](https://hitokoto.cn)（中文补充）
- [PoetryDB](https://poetrydb.org)（英文诗歌）
- 精选内置语料库（各语言分类均有人工整理的长段和短句）

---

## 本地运行

```bash
git clone https://github.com/your-username/auto-quotes.git
cd auto-quotes
# 用浏览器打开 index.html
open index.html        # macOS
start index.html       # Windows
```

> **注意**：部分功能（Wikiquote API、PoetryDB）需要网络连接。内置语料库在离线状态下可用。

---

## 字体说明

本项目使用的字体均经授权确认，可免费商用。文件结构如下：

```
assets/fonts/
  黑体.otf                    ← Noto Sans CJK Light
  CH/
    硬笔.ttf                  ← 平方长安体
    毛笔.ttf                  ← 千图笔锋手写体
    行楷.ttf                  ← 演示夏行楷
  EN/
    AmericanCursive.otf       ← FRBAmericanCursive
    BigSnow.ttf               ← Big Snow
    Signatura.ttf             ← Signatura-Monoline-Script
    Gothic.ttf                ← Holy-Union
  KR/
    Nanum.ttf                 ← Nanum Myeongjo
    NanumPen.ttf              ← Nanum Pen Script
  JP/
    Mincho.ttf                ← 衡山毛筆フォント
    毛笔.ttf                  ← 衡山毛筆行書
    隷书.ttf                  ← 青柳隷書しも
```

> 如需替换或添加字体：在 `index.html` 顶部修改 `@font-face` 路径，并在 JS 中对应语言的 `localFonts` 数组中添加条目。请确认字体授权允许网站嵌入使用（OFL / MIT / Apache 均可）。

---

## 上线部署

### GitHub Pages（免费，推荐）

1. Fork 或 clone 本仓库，推送到你自己的 GitHub
2. 仓库 Settings → Pages → Source 选 `main` 分支
3. 等待约 1 分钟，访问 `https://your-username.github.io/auto-quotes`

---

## 许可证

本项目代码以 [MIT License](LICENSE) 开源。

字体文件版权归各自原作者所有，请在使用前自行确认字体授权协议。

---

## 关于

这是一个 vibe coding 项目，起因是买了一堆彩墨想练字，却每次都找不到值得抄的句子。

如果你也喜欢手帐和练字，欢迎 Star ⭐ 或提 Issue。

---

---

# English

A literary quote generator designed for journaling and calligraphy practice. Supports Chinese, English, Japanese, French, and Korean. Randomly fetches passages from literature, philosophy, poetry, and song lyrics — with font switching for handwriting practice.

🔗 **Live demo:** https://sieg22.github.io/auto-quotes/

---

## Features

- **5 languages**: 中文 / English / 日本語 / Français / 한국어
- **2 length modes**: Long passages (for copying practice) / Short quotes (for journals)
- **Multiple categories**: Literature · Philosophy · Poetry · Lyrics & Scripts · more
- **Font switching**: Load local fonts and switch between them for practice
- **Collection**: Save favourite quotes; double-click any saved quote to restore it
- **Dark mode**: Easy on the eyes
- **UI language toggle**: 中 / En switch in the top-left corner
- **Accent palette**: Subtle warm colour shifts on each new quote
- **Zero dependencies**: Pure HTML + CSS + JS, no build tools, no server needed

---

## Data Sources

- [Wikiquote](https://www.wikiquote.org) (zh / en / ja / fr / ko via MediaWiki API)
- [Hitokoto](https://hitokoto.cn) (Chinese supplement)
- [PoetryDB](https://poetrydb.org) (English poetry)
- Hand-curated pools for all language/category combinations

---

## Quick Start

```bash
git clone https://github.com/your-username/auto-quotes.git
cd auto-quotes
open index.html      # macOS
start index.html     # Windows
```

No build step required. Some features (Wikiquote, PoetryDB) require internet access.

---

## Adding Custom Fonts

1. Place font files in the appropriate folder (`font/CN/`, `font/EN/`, `font/JP/`)
2. Uncomment and fill in the `@font-face` declaration at the top of `index.html`
3. Add an entry to the `localFontsZH` / `localFontsEN` / `localFontsJP` array in the JS

> Please verify that the font licence permits web use (OFL, MIT, Apache, etc.)

---

## Deployment

### GitHub Pages (free, recommended)

1. Push to your GitHub repo
2. Settings → Pages → Source: `main` branch
3. Visit `https://your-username.github.io/auto-quotes` after ~1 min

---

## Licence

Code: [MIT License](LICENSE)

Font files are subject to their respective licences. Please verify before redistribution.
