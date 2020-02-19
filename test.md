#### 1.上传文件

~~~git
touch 1.txt
git add 1.txt
git commit -m'upload 1.txt'
git push -u origin master
~~~

#### 2.更换远程仓库地址

~~~git
git remote -v
git remote rm origin
git remote add origin https://github.com/WJY1225/note
~~~

#### 3.删除远程仓库文件

~~~git
git push origin master
dir
git rm (-r --cached) 1.txt
git commit -m'delete 1.txt'
git push (-u origin master)
~~~

#### 4.删除其他库文件

~~~git
git clone https://github.com/WJY1225/git-demo
cd git-demo
git rm 1.py
git commit -m 'delete 1.py'
git push
~~~





#### Morvan git

```git
'''
name: test_gitTUT.py
author: Wan Jiangyuan
time: 2020.02.03
funcation: create a git TUT and regarding oprations
email: 15611562852.163.com

'''

# cd ~/desktop/gitTUT
# git config --global user.name "WJY"
# git config user.name
# git init
# ls -a
# touch 1.py

# git add 1.py
# git commit -m"change 2"

# git log
# git status -s
# git diff
# git diff --cached
# git diff HEAD

# git log --oneline
# git commit --amend --no-edit

# git reset 1.py            staged-->modified
# git reset --hard HEAD     staged-->modified
# git reset --hard HEAD^    change2-->change1
# git reset --hard HEAD~10  change11-->change1
# git reset --hard 2a17864  return to specific state

# git reflog                change1-->change2
# git reset --hard 2a17864  change1-->change2
# git checkout fe74fa1 -- 1.py  one file back

# git branch dev             create branch but no move
# git checkout -b dev        create branch and move to it
# git branch                 scan branch
# git log --oneline --graph
# git checkout dev           change to branch
# git checkout master
# git branch -d dev          delete branch

# git merge --no-ff -m "keep merge info" dev

# git rebase --continue/abort



# git stash   :happy coding
# git checkout -b boss    :I love boss
# git commit -am"boss job"
# git checkout master
# git merge --no-ff -m "merge boss job" boss
# git commit -am"solve boss conflict"
# git log --oneline --graph
# git branch -D boss
# git checkout dev
# git stash pop


#  git remote add origin https://github.com/WJY1225/git-demo.git
# git push -u origin master
```



