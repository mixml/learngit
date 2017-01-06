# git使用
## 使用github远程库步骤
1、在github上创建项目

2、使用git clone https://github.com/xxxxxxx/xxxxx.git克隆到本地

3、编辑项目

4、git add . （将改动添加到暂存区）

5、git commit -m "提交说明"

6、git push origin master 将本地更改推送到远程master分支。

## 问答
1. 当远程库发生了更改以后，要如何同步到本地库?
  - 答: 使用git pull 命令.
2. 如何回退版本?
  - 答: `git reset --hard HEAD^ `表示回退到上一个版本, `git reset --hard HEAD~10` 表示回退到前10个版本. `git reset --hard xxxxx` 表示回退到xxxxx编号开头的版本.
3. 如何撤销操作?
  - 答: `git check -- filename.txt`
4. 如何删除文件?
  - 答: `git rm filename.txt`
5. 如何查看版本?
  - 答: `git reflog`
6. 如何查看状态?
  - 答: `git status`
7. 如何添加远程库?
  - 答: `ssh-keygen -t rsa -C "youremail@example.com"`, 将`id_rsa.pub`填入github`https://github.com/settings/keys`, 再执行命令`git remote add origin git@github.com:xxxx/xxxx.git`
8. 如何列出一个版本里所有提交的文件?
  - 答: `git ls-files`.
9. 如何提交所有更改过的文件?
  - 答: `git add -A .`
10. 如何提交添加新文件和编辑过的文件但不包括删除的文件?
  - 答: `git add .`
11. 如何添加编辑或者删除的文件，但不包括新添加的文件?
  - 答: `git add -u`
12. 如何修改最后一次commit的信息?
  - 答: `git commit --amend`
  
  
