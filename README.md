# KKbox-Churn-Analysis


# 查看線上庫的地址
$ git remote -v
origin  git@github.com:milalaliu/fork.git (fetch)
origin  git@github.com:milalaliu/fork.git (push)


# 配置上游庫的路徑
$ git remote add upstream ssh.git


# 查看是否添加成功
$ git remote -v
origin  git@github.com:milalaliu/fork.git (fetch)
origin  git@github.com:milalaliu/fork.git (push)
upstream  ssh (fetch)
upstream ssh (push)


# 抓取原倉庫的修改文件
$  git fetch upstream
remote: Enumerating objects: 33, done.
remote: Counting objects: 100% (33/33), done.
remote: Compressing objects: 100% (31/31), done.
remote: Total 33 (delta 11), reused 12 (delta 2), pack-reused 0
Unpacking objects: 100% (33/33), done.
From github.com:JinJieTan/Palantir
* [new branch]      dev            -> upstream/dev
* [new branch]      develop/kk     -> upstream/develop/kk
* [new branch]      develop/nn0917 -> upstream/develop/nn0917
* [new branch]      master         -> upstream/master
* [new branch]      peter          -> upstream/peter


# 切換master分支
$ git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 1 commit.
(use "git push" to publish your local commits)


# 提交
$ git merge upstream/master
$ git push origin master
