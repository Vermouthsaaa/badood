# 模板

这是一个用于 [Hugo 主题 Stack](https://github.com/CaiJimmy/hugo-theme-stack) 的快速启动模板，该模板包含了基础的主题结构和配置。同时已经配置好了 GitHub Actions，可以自动将站点部署到公开的 GitHub Pages。



## 目录

核心文件结构如下：

```bash
project/
│
├── config/_default/          
│   └── config.toml    # 站点核心配置（URL、主题、参数等）
│
├── content/          
│   └── _index.md     # 首页内容（Markdown 格式）
│
├── layouts/         
│   └── index.html    # 首页模板（定义页面结构）
│
└── static/          
    ├── paper.css     # 全局样式文件（控制页面外观，如颜色、字体、布局）
    └── *.png         # 静态资源（图片等）
```



## 快速开始

1. 点击 *Use this template*，并创建你的仓库，例如：`https://<username>.github.io/<repository-name>`
   ![Step 1](https://user-images.githubusercontent.com/5889006/156916624-20b2a784-f3a9-4718-aa5f-ce2a436b241f.png)

2. 在本地调试项目，在终端运行 `hugo server`，即可本地预览网站。
3. 查看 `config` 文件夹中的配置文件，并根据需要进行修改。
   请务必更新 `config/_default/config.toml` 中的 `baseurl`，设置为你的网站地址。
   例如，如果你的仓库名是 `my-blog`，那么 `baseurl` 应该是：`https://<username>.github.io/my-blog/`

3. 完成修改后，提交（commit）并推送（push）代码。
4. 进入仓库的 `Settings` -> `Pages`，将 `Build and deployment` -> `Source` 设置为 `GitHub Actions`。
   ![Change build and deployment source](https://github.com/user-attachments/assets/192459bf-25d8-441e-8029-c108d789e449)
5. GitHub Actions 会自动将站点部署，如果你的仓库名是 `my-blog`，对应的 GitHub Pages：`https://<username>.github.io/my-blog/`
