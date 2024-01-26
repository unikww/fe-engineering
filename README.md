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

- insert_final_newline 用于设置文件是否以一个空白行结尾

`insert_final_newline: true` 的效果如下

<img width="615" alt="截屏2024-01-26 11 33 42" src="https://github.com/unikww/fe-engineering/assets/45612221/33608ba0-034c-4377-bb97-cf079e71ba47">

`insert_final_newline: false` 的效果如下

<img width="615" alt="截屏2024-01-26 11 35 31" src="https://github.com/unikww/fe-engineering/assets/45612221/71a67d0d-1c46-4568-a5dd-28e4d155a032">

- end_of_line 用于设置文本换行的方式

`CRLF: "\r\n"`, windows系统环境下的换行方式

`LF: "\n"`, Linux系统环境下的换行方式

其他没啥区别，与操作系统换行策略有关。如果同一个项目，开发人员使用不同操作系统的编辑器或 IDE 开发，可以统一使用 lf 还是 crlf

## Prettier

## ESLint

## cSpell

## Vitest

说到 [Vitest]() 工具，就要说单元测试。一个单元测试是一段自动化的代码，这段代码调用被测试的工作单元，之后对这个单元的单个最终结果的某些假设进行校验。单元测试几乎都是用单元测试框架编写的；只要产品代码不发生变化，单元测试的结果是稳定的

有很多人认为单元测试就像用一个装鸡蛋的篮子测试能不能装鸭蛋，实际作用并不大。这就引发我们的思考，如何写出有效的单元测试，让其发挥作用更好的服务产品

笔者选用 Vitest 作为本项目的测试框架，在项目中添加 Vitest

```shell
npm i vitest --save-dev
```



