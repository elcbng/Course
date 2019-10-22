# Before all start
>其实最开始做这个的时候，只是想给一小部分人用于存放自己的笔记  
>做着做着就想干脆不如做大一点就好了。               ————子曦

## 这不过是一个Markdown笔记本而已
在这里可以分享你所学知识的笔记

**操作流程：**  
先 fork 这个 repo
```
git clone https://github.com/CerteKim/BNG.git
cd BNG
git checkout pr
```

然后使用任何的工具来 新增，删除，编辑 你想编辑的文件
```
git add .
git commit -m '<描述你的提交>'
```

提交你的文件
```
git push origin pr
```

完成修改之后，前往 github 回到 pr 分支，点击旁边绿色的 Compare & pull request 按钮提交pr

**假如上游更新了：**
```
git checkout master
git pull origin master
git checkout pr
git rebase master # 或者 git merge master
```

如果有冲突请手动解决

### 请遵守原有的文件存放结构