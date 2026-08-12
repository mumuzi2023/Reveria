# 绮梦 · Reveria

> 在星尘落下的地方，故事开始生长。

StoryForge 的品牌与产品介绍站点。当前实现是单页静态网站，不依赖 Generator API。

## 结构

```text
Reveria/
├── index.html              页面、Tailwind CDN 样式和交互脚本
├── assets/                 Hero、图标和 favicon
└── .github/workflows/      GitHub Pages 部署
```

## 本地预览

```bash
python3 -m http.server 8080
```

打开 <http://localhost:8080>。也可以直接打开 `index.html`，但使用静态服务器更接近部署环境。

## 部署

`.github/workflows/deploy.yml` 在仓库更新后发布静态文件到 GitHub Pages。网站没有构建步骤。

## 相关私有仓库

- `gal_generator`：AI 生成后端和创作者工作台。
- `gal_web_runtime`：加载 `game_data.json` 的静态视觉小说播放器。

访问远端链接需要对应私有仓库权限。

## License

Copyright © 2026 mumuzi2023. All Rights Reserved。详见 [LICENSE](LICENSE)。
