<div align="right">
简体中文 | <a href="docs/readme/README.en_US.md">English</a> | <a href="docs/readme/README.ja.md">日本語</a>
</div>

<h1 align="center">hikoutai-stamp</h1>
<p align="center">航空自卫队公开照片风格的图片标注工具</p>

<div align="center">

[![星标](https://img.shields.io/github/stars/PiggyWu981/hikoutai-stamp?style=for-the-badge&color=orange&label=%E6%98%9F%E6%A0%87)](https://github.com/PiggyWu981/hikoutai-stamp/stargazers)
[![最近提交](https://img.shields.io/github/last-commit/PiggyWu981/hikoutai-stamp?style=for-the-badge&color=blue&label=%E6%9C%80%E8%BF%91%E6%8F%90%E4%BA%A4)](https://github.com/PiggyWu981/hikoutai-stamp/commits/master)
[![在线演示](https://img.shields.io/badge/%E5%9C%A8%E7%BA%BF%E6%BC%94%E7%A4%BA-4c9a42?style=for-the-badge)](https://piggywu981.github.io/hikoutai-stamp/)
[![单文件](https://img.shields.io/badge/%E5%8D%95%E6%96%87%E4%BB%B6-d4a84b?style=for-the-badge)](index.html)
[![零依赖](https://img.shields.io/badge/%E9%9B%B6%E4%BE%9D%E8%B5%96-6e7681?style=for-the-badge)](index.html)
[![Gitee 镜像](https://img.shields.io/badge/Gitee%20%E9%95%9C%E5%83%8F-c71d23?style=for-the-badge)](https://gitee.com/PiggyWu981/hikoutai-stamp)
[![许可证](https://img.shields.io/badge/%E8%AE%B8%E5%8F%AF%E8%AF%81-GPL--3.0-blue?style=for-the-badge)](LICENSE)

</div>

## 简介

hikoutai-stamp 是一款基于浏览器的图片标注工具，可在任意照片上叠加与航空自卫队公开照片相同版式的「対象機」标签条以及右下角摄影署名，并将结果导出为 PNG 图片。

处理流程基于 HTML5 Canvas 在浏览器本地完成，图片不会上传至任何服务器，无需后端服务。工具操作界面为日语。

## 特性

- 支持独立控制顶部标签条与右下角署名的显示与隐藏
- 标签及署名文言可自由编辑，内置 Y-9、H-6、Su-27、B-52H、RC-135 五种预设
- 提供深色（黑底白字）与浅色（白底黑字）两种主题
- 基于 Canvas 的实时预览，参数调整即时生效
- 支持导出 PNG，依次尝试系统分享（Web Share）、直接下载、全屏预览三种保存方式，兼容移动端浏览器
- 支持点击或拖拽选择 JPG、PNG、WebP 格式图片
- 全部处理均在本地完成，不依赖任何服务端
- 单文件实现（`index.html`），无需构建，无第三方运行时依赖
- 响应式布局，适配桌面与移动设备

## 在线使用

直接访问 [https://piggywu981.github.io/hikoutai-stamp/](https://piggywu981.github.io/hikoutai-stamp/) 即可使用，无需安装任何软件。

## 本地运行

```bash
git clone https://github.com/PiggyWu981/hikoutai-stamp.git
cd hikoutai-stamp
python -m http.server 8000
```

浏览器访问 `http://localhost:8000`。也可直接打开 `index.html`；「系统分享」等能力需要 HTTPS 或 localhost 环境。

## 使用方法

1. 点击虚线区域或将图片拖入页面，选择 JPG、PNG 或 WebP 格式的图片。
2. 在左侧面板中编辑顶部标签文言与右下角署名，可点击预设按钮快速填充常用机型描述。
3. 选择深色或浅色主题，并通过复选框控制标签与署名的显示。
4. 点击「PNG を保存」导出图片。

## 注意事项

> **注意**
>
> - 本工具仅用于模仿航空自卫队公开照片的版式风格，适用于学习、交流等非正式场景。
> - 请勿将输出图片用于伪造官方发布资料、误导公众或其他不当用途。
> - 预设文言中的机型及「初めて確認した」等表述均为示例内容，不代表任何真实事件。

## 许可证

本仓库暂未指定开源协议，当前不包含 LICENSE 文件。

## 致谢

- 字体：[Noto Sans JP](https://fonts.google.com/noto/specimen/Noto+Sans+JP)、Noto Sans SC（Google Fonts）
- 版式参考：航空自卫队公开照片的排版风格

## 相关链接

- [在线演示](https://piggywu981.github.io/hikoutai-stamp/)
- [GitHub 仓库](https://github.com/PiggyWu981/hikoutai-stamp)
- [Gitee 仓库（镜像）](https://gitee.com/PiggyWu981/hikoutai-stamp)
