# hugoDocs
自训练系统的操作文档

## 基本手册

### 如何在线编辑或添加文档页面

要编辑或添加文档，你需要拥有一个 [GitHub](https://github.com/login) 账户。要修改文档文件或添加文档页面，只需在要编辑的页面上点击 `Edit this page`。如果需要添加子页面，请点击 `Create child page`。

如果需要编辑带有 [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) 标记的文本，请点击 `Fork this repository` 按钮。

阅读如何编辑GitHub文件的更多信息，请参阅 [GitHub文档](https://docs.github.com/en/github/managing-files-in-a-repository/editing-files-in-another-users-repository)。

请注意，文件具有标记以正确显示在站点上：标题、链接标题、权重（影响侧边栏文件显示顺序）和描述（可选）：

```yaml
---
title: "标题"
linkTitle: "链接标题"
weight: 1
description: >
    描述
---
```

### 如何在本地启动站点

#### 安装

1. 安装 Hugo

获取 [v110.0-extended版的Hugo发布版](https://github.com/gohugoio/hugo/releases/tag/v0.110.0)。 在GitHub发布版的Assets部分展开，滚动到**Extended**版本的列表。 [了解更多](https://gohugo.io/getting-started/installing/#quick-install)

将 `hugo` 的路径添加到 `PATH` 环境变量中。

1. 获取 Docsy 主题代码

```bash
git submodule update --init --recursive
```

1. 安装 Docsy 主题依赖项

为了构建或更新站点的 CSS 资源，你需要安装几个包。 为了安装它们，你必须在你的机器上安装一个最新版本的 [NodeJS](https://nodejs.org/en/)（测试使用 v18.0）。你可以直接使用 [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) 安装，或者通过像 [nvm](https://github.com/nvm-sh/nvm) 这样的环境管理器。 默认情况下，`npm` 在你运行 `npm install` 的目录下安装工具。

```bash
(cd site/ && npm install)
```

完整的文档可在 [这里](https://www.docsy.dev/docs/get-started/other-options/#for-an-existing-site) 查看。



### 外网部署

[github Pages部署hugo](https://gohugo.io/hosting-and-deployment/hosting-on-github/)



详情参阅[docsy主题](https://gohugo.io/hosting-and-deployment/hosting-on-github/)

