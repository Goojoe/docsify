# 5.githubpages部署
由于我自己出现了git push 无法输入密码的尴尬情况，所以我推荐SSH部署
其他的大家可以自行Google/baidu
## 5.1Windows创建SSH秘钥
### 5.1.1自己找.ssh文件
```markdown
C:\Users\你的管理员账户\.ssh
```
若没有.ssh文件可以自己新建一个
### 5.1.2Everything搜索
Everything搜索.ssh

## 5.2创建RSA秘钥
在.ssh目录下
右键打开Git bash
输入以下命令一直回车即可
```bash
ssh-keygen -t rsa
```

![image-20211110194038104](https://cdn.jsdelivr.net/gh/Goojoe/picgo/docsify/ssh.png)

会生成两个文件
`id rsa`私钥，绝对不能泄露
`id rsa pub`公钥，记事本打开复制，等会会用到


