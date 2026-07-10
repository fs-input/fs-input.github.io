# 风水形音输入法

**Geomancy Form-Phonetic Input Method**

> 迅疾如风、流畅若水 · V 1.3.1（2026.07.08 更新词库）

![风水字根表](assets/images/roots-table.png)

一款简体中文输入法，以"**米人**"字形字根布局为基础，融合"易经""阴阳五行"学说与英语字母象形。形码为主、音码为补——易学易记、输入迅捷。

## 特性

- 覆盖《通用规范汉字表》全部 **8105** 个汉字
- **15.7 万条**词库
- 26 键"米人"字根布局，按风水排布
- 拆字简单，没有难拆字
- 形码为主，音码为补
- 三级候选词，精准输入，全键盘掌控

## 快速开始

### 1. 安装 Rime
下载并安装 [Rime](https://rime.im/download/)（Windows 用小狼毫 Weasel，macOS 用鼠须管 Squirrel，Linux 用 ibus-rime / fcitx-rime）。

### 2. 下载风水方案
下载最新发布包 —— **[Releases](https://github.com/fs-input/fs-input.github.io/releases)** —— 并解压，内含 5 个文件：

| 文件 | 说明 |
|---|---|
| `default.yaml` | Rime 默认设置 |
| `geomancy.schema.yaml` | 风水方案定义 |
| `geomancy.dict.yaml` | 15.7 万词库 |
| `geomancy.extended.dict.yaml` | 用户自定义词库 |
| `weasel.yaml` | Windows（小狼毫）界面设置 |

### 3. 部署
将 5 个文件复制到 Rime 用户数据目录，然后**重新部署** Rime：

- **Windows（小狼毫）：** `%APPDATA%\Rime\`
- **macOS（鼠须管）：** `~/Library/Rime/`
- **Linux：** `~/.config/ibus/rime/` 或 `~/.local/share/fcitx5/rime/`

### 4. 选择方案
打开 Rime 输入法设定，选择 **风水形音**。

> 含截图的完整安装指引：[安装教程](https://fs-input.github.io/zh/appendix-a-install)

## 教程（10 种语言）

含 8105 字拆解实时查询的交互式教程：

| | | | |
|---|---|---|---|
| [中文](https://fs-input.github.io/) | [English](https://fs-input.github.io/en/) | [Español](https://fs-input.github.io/es/) | [Français](https://fs-input.github.io/fr/) |
| [العربية](https://fs-input.github.io/ar/) | [Русский](https://fs-input.github.io/ru/) | [Deutsch](https://fs-input.github.io/de/) | [日本語](https://fs-input.github.io/ja/) |
| [Tiếng Việt](https://fs-input.github.io/vi/) | [한국어](https://fs-input.github.io/ko/) | | |

## 链接

- **方案压缩包：** [Releases](https://github.com/fs-input/fs-input.github.io/releases)
- **教程网站：** https://fs-input.github.io
- **组织主页：** https://github.com/fs-input

## 致谢

- **作者：** 詹小虫
- 基于 [Rime](https://rime.im/) 与 [Just the Docs](https://github.com/pmarsceill/just-the-docs) 主题构建。
- 76 个自创字根字符（Unicode PUA 区）由内嵌的 `EUDC.ttf` 渲染。

---

[English](README.md)
