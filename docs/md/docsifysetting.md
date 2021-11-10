# 3.docsify设置
## 3.1 侧边栏标题及右上角GitHub跳转
编辑index.html

```html
window.$docsify = {
      name: 'docsify指南',
      repo: 'https://github.com/Goojoe/docsify',
}
```

将name改为你想要的标题

repo填写你的GitHub仓库链接

保存后就是这样,左边就是name,右边就是跳转到上面填的repo仓库链接

![image-20211110150924181](https://cdn.jsdelivr.net/gh/Goojoe/picgo/docsify/Sidebargithub.png)





## 3.2多页文档

你现在在docs里编辑文档,为了归纳md文件,你可以创建任意文件夹

例:我创建了一个md文件夹,并在md**文件夹内**新建了1.md

那么引用此文档的代码就是

```markdown
[标题](md/1.md)
```

文件树

```markdown
docs
├──md
	├──1.md
```



## 3.2启用侧边栏

编辑index.html

```html
window.$docsify = {
      name: 'docsify指南',
      repo: 'https://github.com/Goojoe/docsify',
      loadSidebar: true,
      
}
```

添加`loadSidebar: true,` 逗号是为了添加其他配置不冲突

### 3.2.1侧边栏文档

接着创建 `_sidebar.md` 文件，内容如下

```markdown
<!-- docs/_sidebar.md -->

* [首页](zh-cn/)
* [指南](zh-cn/guide)
```

