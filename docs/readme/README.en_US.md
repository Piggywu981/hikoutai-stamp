<div align="right">
<a href="../../README.md">简体中文</a> | English | <a href="README.ja.md">日本語</a>
</div>

<h1 align="center">hikoutai-stamp</h1>
<p align="center">A photo annotation tool in the style of Japan Air Self-Defense Force public-release photographs</p>

<div align="center">

[![Stars](https://img.shields.io/github/stars/PiggyWu981/hikoutai-stamp?style=for-the-badge&color=orange&label=stars)](https://github.com/PiggyWu981/hikoutai-stamp/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/PiggyWu981/hikoutai-stamp?style=for-the-badge&color=blue&label=last%20commit)](https://github.com/PiggyWu981/hikoutai-stamp/commits/master)
[![Online Demo](https://img.shields.io/badge/online%20demo-4c9a42?style=for-the-badge)](https://piggywu981.github.io/hikoutai-stamp/)
[![Single File](https://img.shields.io/badge/single%20file-d4a84b?style=for-the-badge)](index.html)
[![Zero Dependency](https://img.shields.io/badge/zero%20dependency-6e7681?style=for-the-badge)](index.html)
[![Gitee Mirror](https://img.shields.io/badge/Gitee%20mirror-c71d23?style=for-the-badge)](https://gitee.com/PiggyWu981/hikoutai-stamp)

</div>

## Introduction

hikoutai-stamp is a browser-based photo annotation tool. It overlays a "Target Aircraft" (対象機) bar at the top and a photo credit at the bottom right of any image, following the layout of Japan Air Self-Defense Force (JASDF) public-release photographs, and exports the result as a PNG file.

All processing runs locally in the browser via HTML5 Canvas. Images are never uploaded to any server, and no backend is required. The user interface is in Japanese.

## Features

- Independently toggle the top label bar and the bottom-right credit
- Fully editable label and credit text, with five built-in presets: Y-9, H-6, Su-27, B-52H, RC-135
- Two themes: dark (white text on black) and light (black text on white)
- Real-time Canvas preview; changes apply immediately
- PNG export with three fallback save paths — Web Share, direct download, and a full-screen preview — for compatibility with mobile browsers
- Select images by click or drag-and-drop (JPG, PNG, WebP)
- Entirely client-side; no server required
- Single-file implementation (`index.html`): no build step, no runtime dependencies
- Responsive layout for desktop and mobile devices

## Online Usage

Open [https://piggywu981.github.io/hikoutai-stamp/](https://piggywu981.github.io/hikoutai-stamp/) in a browser — no installation required.

## Local Setup

```bash
git clone https://github.com/PiggyWu981/hikoutai-stamp.git
cd hikoutai-stamp
python -m http.server 8000
```

Then open `http://localhost:8000`. Opening `index.html` directly also works; features such as Web Share require an HTTPS or localhost context.

## How to Use

1. Click the dashed area or drag an image (JPG / PNG / WebP) onto the page.
2. Edit the top label and bottom-right credit in the left panel; preset chips fill in common aircraft descriptions.
3. Choose the dark or light theme and toggle label/credit visibility with the checkboxes.
4. Click "PNG を保存" (Save PNG) to export.

## Disclaimer

> **Disclaimer**
>
> - This tool is intended solely for imitating the layout style of JASDF public-release photographs, for informal purposes such as study and personal use.
> - Do not use the output images to fabricate official publications, mislead the public, or for any other improper purpose.
> - Aircraft types and phrasings such as "初めて確認した" in the presets are examples only and do not represent real events.

## License

This repository does not currently specify an open-source license; no LICENSE file is included.

## Acknowledgments

- Fonts: [Noto Sans JP](https://fonts.google.com/noto/specimen/Noto+Sans+JP), Noto Sans SC (Google Fonts)
- Layout reference: JASDF public-release photograph layout

## Links

- [Live Demo](https://piggywu981.github.io/hikoutai-stamp/)
- [GitHub Repository](https://github.com/PiggyWu981/hikoutai-stamp)
- [Gitee Repository (mirror)](https://gitee.com/PiggyWu981/hikoutai-stamp)
