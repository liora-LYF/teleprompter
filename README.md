# 《刘易肥一气之下做了个提词器》GitHub Pages

这是一个可直接部署到 GitHub Pages 的静态版本。

## 目录说明

```text
index.html   # 完整提词器，GitHub Pages 首页
.nojekyll    # 告诉 GitHub Pages 跳过 Jekyll
LICENSE      # MIT
README.md
```

`index.html` 是完全独立的单文件应用：CSS、JavaScript、图标全部内联，没有外部 CDN、字体、图片或接口依赖。

## 部署步骤

1. 在 GitHub 新建一个公开仓库，例如 `teleprompter`。
2. 进入仓库，点击 **Add file → Upload files**。
3. 把本目录中的 `index.html` 上传到仓库**根目录**。
   - 文件名必须是 `index.html`，不能放到子目录中。
   - `.nojekyll` 也建议一起上传；它是空文件。
4. 打开仓库 **Settings → Pages**。
5. **Build and deployment → Source** 选择 **Deploy from a branch**。
6. 分支选择 **main**，目录选择 **/ (root)**，点击 Save。
7. 等待几十秒，访问：

```text
https://你的GitHub用户名.github.io/仓库名/
```

如果仓库名是 `你的用户名.github.io`，则直接访问：

```text
https://你的用户名.github.io/
```

## 分享给朋友

把上面生成的 GitHub Pages 网址发给朋友即可。对方直接打开使用，不需要安装 Skill、Node.js 或任何依赖。

如果朋友在微信等内置浏览器里无法全屏，建议使用“在浏览器中打开”，选择 Chrome、Edge 或 Safari。

## 数据说明

- 文案和设置保存在访问者自己的浏览器 `localStorage` 中。
- 不会上传到 GitHub，也不会同步给其他访问者。
- 每个访问者打开后都是一份独立的本地提词器。

## 注意

- GitHub 仓库页面本身不是网页应用，必须启用 Pages 后分享 Pages 地址。
- 不建议分享 GitHub 的 raw 文件链接；raw HTML 通常以文本形式打开，而不是运行应用。
- 首次打开时，全屏能力由浏览器决定；点击「全屏提词」即可进入。
