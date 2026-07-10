# Fengshui Form-Phonetic Input Method

**风水形音输入法** · Geomancy Form-Phonetic Input Method

> *Swift as wind, fluid as water.* · V 1.3.1 (dictionary updated 2026.07.08)

![Fengshui radical table](assets/images/roots-table.png)

A Simplified Chinese input method built on the **米 (rice) / 人 (person)** glyph radical layout, weaving together the *I Ching*, *Yin-Yang and the Five Elements* with alphabetic pictography. Form codes form the backbone; phonetic codes act as a supplement — easy to learn, fast to type.

## Features

- Covers all **8,105** characters of the *Table of General Standard Chinese Characters*
- A dictionary of **157,000 words**
- 26-key **米 / 人** radical layout arranged by Feng Shui
- Simple decomposition — no hard-to-split characters
- Form codes as the backbone, phonetic codes as the supplement
- Three tiers of candidate words; precise, full-keyboard input

## Quick Start

### 1. Install Rime
Download and install [Rime](https://rime.im/download/) (Weasel on Windows, Squirrel on macOS, ibus-rime / fcitx-rime on Linux).

### 2. Download the Fengshui schema
Grab the latest package — **[Releases](https://github.com/fs-input/fs-input.github.io/releases)** — and unzip it. It contains 5 files:

| File | Description |
|---|---|
| `default.yaml` | Default Rime settings |
| `geomancy.schema.yaml` | The Fengshui schema definition |
| `geomancy.dict.yaml` | The 157,000-word dictionary |
| `geomancy.extended.dict.yaml` | User custom dictionary |
| `weasel.yaml` | Windows (Weasel) interface settings |

### 3. Deploy
Copy all 5 files into your Rime user data directory, then **redeploy** Rime:

- **Windows (Weasel):** `%APPDATA%\Rime\`
- **macOS (Squirrel):** `~/Library/Rime/`
- **Linux:** `~/.config/ibus/rime/` or `~/.local/share/fcitx5/rime/`

### 4. Select the schema
Open Rime's schema selector and choose **风水形音 (Fengshui)**.

> Full step-by-step guide with screenshots: [Installation tutorial](https://fs-input.github.io/en/appendix-a-install)

## Tutorial (10 languages)

Interactive tutorials with a live-filtered decomposition lookup for all 8,105 characters:

| | | | |
|---|---|---|---|
| [中文](https://fs-input.github.io/) | [English](https://fs-input.github.io/en/) | [Español](https://fs-input.github.io/es/) | [Français](https://fs-input.github.io/fr/) |
| [العربية](https://fs-input.github.io/ar/) | [Русский](https://fs-input.github.io/ru/) | [Deutsch](https://fs-input.github.io/de/) | [日本語](https://fs-input.github.io/ja/) |
| [Tiếng Việt](https://fs-input.github.io/vi/) | [한국어](https://fs-input.github.io/ko/) | | |

## Links

- **Schema package:** [Releases](https://github.com/fs-input/fs-input.github.io/releases)
- **Tutorial site:** https://fs-input.github.io
- **Organization:** https://github.com/fs-input

## Credits

- **Author:** 詹小虫 (Zhan Xiaochong)
- Built on [Rime](https://rime.im/) with the [Just the Docs](https://github.com/pmarsceill/just-the-docs) theme.
- The 76 custom radical glyphs (Unicode PUA area) are rendered by the embedded `EUDC.ttf`.

---

[中文说明](README_CN.md)
