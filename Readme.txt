Git is a version control system.
Git is a free software.
Use VScode commit.

git init
git add
git commit -m "information"

git status
git diff filename
git diff HEAD -- filename


-----------------------版本库--------------------------------------------
                                         |                           |
                                 git diff --cached           |
                                         |                           |
-------------暂存区----------------------              git diff HEAD
                        |                                            |
                     git diff                                |
                        |                                            |
-----工作区--------------------------------------------------------------



git log --pretty=oneline
git ref log
git reset --hard commit_id
git reset HADE filename 撤销暂存区修改

工作区 版本库（暂存区 分支和指向其的指针）

git checkout -- filename 回到最近一次 add 或者 commit
git checkout 分支名称 切换分支

git rm

$ ssh-keygen -t rsa -C "youremail@example.com" 生成SSH

配置SSH到GitHub网站 添加仓库

git remote add origin git@github.com:用户名/仓库名.git

git push -u origin master

//测试 git config --global credential.helper store 避免多次输入账号密码

{
        touch .git-credentials
        vim .git-credentials
        https://{username}:{password}@github.com
}

