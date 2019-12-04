# 百度ai

https://ai.baidu.com/support/news?action=detail&id=1603


### github 步骤

```bash
# 1. 初始化本地仓库
$ git init 

Initialized empty Git repository in /Users/xxx/Desktop/other/baiduai/.git/

# 2. 查看当前git当前状态
# 有红色，说明还有没有被加入缓存区的文件，即未被跟踪
$ git status 

On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        README.md
        index.html
        reset.css

nothing added to commit but untracked files present (use "git add" to track)


# 3. 将修改后的所有(.)文件，加入暂存区
$ git add . 


# 4. 查看当前git状态  红色代表刚刚修改过得文件，绿色代表已经加入暂存区的文件
git status 


On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   README.md
        new file:   index.html
        new file:   reset.css

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md


# 5. 将暂存区的文件 提交到git管理仓库 ，语法：git commit -m '备注消息'
# commit 是提交的意思，只提交蓝色的文件，也就是说只提交暂存的文件
$ git commit -m '创建index.html文件'

[master (root-commit) 938f977] 创建index.html文件
 3 files changed, 87 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.html
 create mode 100644 reset.css
```