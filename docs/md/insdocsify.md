# 2.安装docsify

## 2.1切换npm镜像源

切换淘宝源
打开cmd输入下面命令
```cmd
npm config set registry=https://registry.npm.taobao.org/
```

查询是否成功

```cmd
npm config get registry
```
输出为下面即为修改成功

![image-20211110002459967](https://cdn.jsdelivr.net/gh/Goojoe/picgo/docsify/mirror.png)


## 2.2安装docsify

```cmd
npm i docsify-cli -g
```

## 2.3初始化项目
在你想放docsify项目的地方打开cmd
或者Shift+鼠标右键-->打开powershell
```bash
docsify init ./docs
```

会生成初始化需要的文件

初始化成功后，可以看到 `./docs` 目录下创建的几个文件

- `index.html` 入口文件
- `README.md` 会做为主页内容渲染
- `.nojekyll` 用于阻止 GitHub Pages 忽略掉下划线开头的文件

直接编辑 `docs/README.md` 就能更新文档内容，当然也可以[添加更多页面](https://docsify.js.org/#/zh-cn/more-pages)。

## 2.4实时预览更改
docs文件夹外
```bash
docsify serve docs
```
