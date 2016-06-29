# 《成为创客》

https://tsinghuahigh.github.io/ [![Build Status](https://travis-ci.org/TsinghuaHigh/become-a-maker.svg?branch=master)](https://travis-ci.org/TsinghuaHigh/become-a-maker)

这是一本正在合作撰写中的电子书(divide-and-conquer法)，面向大学/中学生还有对于创客感兴趣的成人。其中[创客课和学校社团](schools/intro.md)这一章还会可以给对创客感兴趣的学校/老师/学生社团看。  
为什么要写这本书？因为其中的作者在开创客课开了四年了，感觉需要把经验知识传播出去啊，否则影响的人太少。另外要是多一些被动收入也不错。  

如果要将此书用于商业用途，请联系作者。

TODO:

- [x] 建立gitbook，上传到github上
- [x] 书籍目录结构
- [x] 定出整体书籍的思路（把成为创客进阶和网游升级进行类比，做导读，而不是大而全）
- [X] 用travis自动编译到gh_pages(大概需要花三四个小时吧) https://gist.github.com/domenic/ec8b0fc8ab45f39403dd
- [ ] 列出各个章节的提纲，技能和副本(截止日期7月15日)
- [ ] 采访各个职业的顶级人才，最好能够招募进来一起做这件事情
- [ ] 列出作者感觉吃力的章节(很明显除了产品经理以外的所有好不好)，找到解决方案
- [ ] 思考商业模式（最简单就是加上捐款链接，或者未来出纸板书，不会有太多钱。显然电子书收费在国内不现实，但是或许可以跟在行、知乎、网易公开课、mooc，众筹网站有什么增值服务/引流合作？或者是部分内容隐藏进行增值服务的收费？）
- [ ] 找一个好的插画师帮忙加插画
- [ ] 找各个可以在线学习的网站和资源，引导学生去那里学习
- [ ] 开始正式撰写每一章，最好有一个编辑天天来催稿！外加审阅和校对。
- [ ] 未来，运营微信公众号？(我觉得最可行的就是经常加新的挑战)
- [ ] 脑洞，如果每一个章节都有一个人物，加上背景故事，会不会更有意思呢？
- [ ] 脑洞，在线做题


本书用gitbook构建，gitbook版本：{{ gitbook.version }}

## 下载安装到本机

### Mac安装+预览方法：

1. 下载以下软件
    * [Homebrew](http://brew.sh/) 在命令行里运行：`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
    * [node](http://nodejs.org/) 在命令行里运行：`brew install nodejs`
    * [gitbook](https://www.gitbook.com/) 在命令行里运行：`sudo npm install gitbook-cli -g`  管理员权限要的是当前mac用户的密码
    * 推荐下载git可视化[sourcetree](https://www.sourcetreeapp.com/)
    * 推荐下载编辑器[atom](http://atom.io/)
2. 下载书籍 `$ git clone https://github.com/TsinghuaHigh/become-a-maker.git` (前提是已经加入到这个项目里了,这里输入的是github的用户名密码)
3. 在书的目录下（有book.json的那个目录）安装插件 `$ gitbook install`
4. 本地预览 `$ gitbook serve`
5. 打开浏览器 http://localhost:4000

### Windows安装+预览方法：

1. 下载以下软件
  * [nodejs](https://nodejs.org/en/)
  * [tortoisegit](http://tortoisegit.org/download/)
  * [git](https://git-for-windows.github.io/)
  * 推荐下载编辑器[atom](https://atom.io/)
2. 通过tortoisegit拉取代码（在目录里右键git clone）地址为：`https://github.com/TsinghuaHigh/become-a-maker.git` 注意要先让项目负责人开通自己的github账号的查看/修改权限。
3. 安装gitbook，命令行里运行`npm install gitbook-cli -g`
4. 切换到项目的目录里（用cd）然后安装插件`gitbook install`
5. 本地预览 `$ gitbook serve`
6. 打开浏览器 http://localhost:4000


### 安装后预览方法：

1. 本地预览 `$ gitbook serve`
2. 打开浏览器 http://localhost:4000

自定义端口号: `$ gitbook serve -p 8080` 默认是4000


### 导出为文件方法

保存为静态网站： `$ gitbook build .`  （一定要注意里面的.，会发布到_build目录底下）

保存为pdf：使用`gitbook-pdf` 可能会有bug，请参考这个网站 http://blog.csdn.net/xiaocainiaoshangxiao/article/details/46882921

## 项目的目录结构

* `book.json` 文档配置文件
* `summary.md` 目录树
* `intro.md` 序言
* `license.md` 版权声明
* `readme.md` 有关书的什么

## Markdown的规范

![Markdown语法](http://images.cnitblog.com/i/46653/201406/211438200988939.png)

另外可以看这个说明：http://www.jianshu.com/p/1e402922ee32/

## Gitbook特有的语法

* 页面中插入一个目录导览：`<!- - toc -->` （注意：去掉横线之间的空格）
* 页面中插入其他页面：`{% include "SUMMARY.md" %}`

## 如何用git进行协作

* 基本指令
    * `git add -A` 把目录下所有未跟踪的文件进行跟踪
    * `git commit -m "See changelog 1.1"` 保存存盘点
    * `git pull` 拉取云端最新的代码
    * `git push` 将最新存盘点推到云端（请保证已经拉去最新的代码）
    * `git status` 查看当前修订状态
* 简单攻略：http://www.bootcss.com/p/git-guide/
* 动手操作的攻略：http://pcottle.github.io/learnGitBranching/?demo
* git 指令清单：http://www.ruanyifeng.com/blog/2015/12/git-cheat-sheet.html
* 复杂攻略：http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/

## 贡献者

* @tianshuo (脑洞大，笑点低，拖延症)
