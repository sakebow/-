# 说明
单纯的为了记录解决冲突的方法，上次学会的已经忘掉了

## 第一步，在GitHub网站上创建一个带有README.md的远程代码库！
```bash
git pull <remote> <branch>
# 使用 pull 语句，加上远程库名称，加上分支，就能拿到远程库的所有内容
```

## 第二步，创建新文件practice.js，并随意写一点东西，推上去！
```bash
touch practice.md
# git的命令行有很多和Linux类似的命令，可以直接使用
```

然后打开文件写下这些东西：

```javascript
var index = document.getElementById('#index')
```

看起来没有什么问题。好的！推上去！

```bash
git add . # 添加所有文件
git commit -m <comments> # 提交修改
git push -u <remote> <branch> # 推到远程代码库
```

## 第三步，修改他！
有一天，你觉得这个方法不行，或者说别人拿枪指着你逼你改

好嘛，改嘛

```javascript
let index = $('#index')
```

提交！

没有报错。似乎没有什么问题。

## 第四步，删掉他！
最终，项目崩盘了；或者说你可以大卖一笔，决定把开源的东西删掉

```bash
rm practice.js
```

提交！

没有报错！到此为止一直都没有报错！没有任何冲突错！