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



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