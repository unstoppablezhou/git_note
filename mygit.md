## git+typora作为笔记使用

创建一个空的笔记目录，右键git bush打开，输入命令连接你想要的库的 https: 链接

```git
git clone https://github.com/unstoppablezhou/notes.git
```

接下来使用命令进入创建的目录

```git
cd notes
```

再用命令

```git
git status
```

最后创建git目录记录git相关笔记，github目录记录相关笔记等

```git
mkdir git
mkdir github
```

进入相关目录下创建文件，把git目录直接拖到typora里面编辑

```git
cd git
touch mygit.md
```

编辑完了后上传github

```git
git add .
git commit -m "add all"
git push
```



git提交到github最后一步git push发生错误，原因是github上的文件目录结构与本地不同，这时需要将它们合并后重新提交。这里需要注意的是合并命令需要vpn翻墙，不然连不上，main跟master是一个意思，主要看你库里的是哪个词

```
git pull --rebase origin main

git push origin main
```



在git提交时第二部git commit -m “xx” 出错，可能是你的本地项目与github上的项目分支(main)不同，需要另建一个分支提交，最后合并分支，删除新创建的分支