# Git指令集合

1. cd +路径

2. mkdir + 文件夹名

3. git init

4. ls -al

5. touch + 文件名

6. vi + 文件名

   vi编辑的指令

   1. p开始输入
   2. esc结束输入
   3. 输入：wq保存并返回到命令行

7. cat + 文件名

8. git status

9. git log

10. git log --pretty=oneline

11. git reflog

12. git add 文件名

13. git commit -m "备注"

14. git reset --hard HEAD~k //k为数字，表示从当前版本开始，回到前k个版本

15. git reset --hard 版本号//回到该版本

16. get checkout -- 文件名//丢弃工作区中该文件的改动

17. get reset HEAD 文件名//把文件从暂存区拉回到文件区

18. git differ HEAD -- 文件名

19. git differ HEAD~1 HEAD -- 文件名

20. rm 文件名

21. git restore -- 文件名

22. git rm 文件名

## Git分支管理

1. 查看分支：`git branch`
2. 创建分支：`git branch <name>`
3. 切换分支：`git checkout <name>`
4. 创建+切换分支：`git checkout -b <name>`
5. 合并某分支到当前分支：`git merge <name>`
6. 删除分支：`git branch -d <name>`
7. 为紧急处理新的需求，保存当前分支正在处理的信息：git stash
8. 结束新的需求后，查看之前保存的分支信息：git stash list
9. 回复到之前保存的分支信息：git stash pop

## 使用Github

1. 创建一个GitHub仓库

2. 添加SSH账户

   1. 个人信息的setting中找到

   2. 在个人电脑的主目录下打开git bush，然后编辑 vi .gitconfig，修改该机器的git配置，填写GitHub账号名和邮箱地址

      <img src="D:\Application\TyporaPicture\image-20220626221925791.png" alt="image-20220626221925791" style="zoom:50%;" />

   3. 将SSH和邮箱绑定：<img src="D:\Application\TyporaPicture\image-20220626222102921.png" alt="image-20220626222102921" style="zoom:50%;" />

   4. 将其中的公钥输入到Github网页的SSH当中去即可。<img src="D:\Application\TyporaPicture\image-20220626222232728.png" alt="image-20220626222232728" style="zoom:50%;" />

3. 克隆项目

   1. <img src="D:\Application\TyporaPicture\image-20220626222336628.png" alt="image-20220626222336628" style="zoom:67%;" />
   2. 然后找到要下载的路径下打开git bush，输入git clone 地址  即可。

4. 上传分支

   1. 分支修改好后，通过"git push origin 分支名"   进行上传

5. 拉取分支

   1. git pull orgin 分支名

[Git教程链接](https://www.jb51.net/article/191350.htm#_label5)