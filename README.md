# 搭建完整的前端工程化工作流

本仓库旨在提供一个完整的前端工程化工作流

这套模版的由 Vite + EditorConfig + Prettier + ESLint + cSpell + commitlint

## Vite

[Vite](https://vitejs.dev/) 是新一代的前端构建工具，主要利用浏览器 ESM 特性导入组织代码，在服务器端按需编译返回，完全跳过了打包这个概念

直接在电脑上创建一个新项目

```shell
mkdir react-starter && npm init -y
```

上面的步骤成功后，接着安装 `vite`

```shell
npm i vite --save-dev
```

然后在根目录依次添加 `index.html`、`main.js` 等文件，目录文件如下

![目录文件](https://github.com/unikww/fe-engineering/assets/45612221/640631e1-158b-4825-abce-8e422bac0b86)

在终端中运行下面的命令

```shell
npm run dev
```

在浏览器地址栏输入 http://localhost:5173/ 就可以正常访问

一个非常简单的 Vite 小项目正常运行起来，接下来为这个小项目加入各种工具，使它能胜任任何业务开发

## EditorConfig

[EditorConfig](https://editorconfig.org/) 有助于跨不同编辑器和 IDE 处理同一项目的多个开发人员保持一致的编码风格。

通过 EditorConfig 的重要配置项解释如何保持一致的编码风格

- end_of_line 用于设置文本换行的方式

`CRLF: "\r\n"`, windows系统环境下的换行方式

`LF: "\n"`, Linux系统环境下的换行方式

其他没啥区别，与操作系统换行策略有关。如果同一个项目，开发人员使用不同操作系统的编辑器或 IDE 开发，可以统一使用 lf 还是 crlf

## Prettier

## ESLint

## cSpell
