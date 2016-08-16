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
