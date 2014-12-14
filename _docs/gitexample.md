---
layout: docs
title: Git Examples
prev_section: bashexample
next_section: tclexample
permalink: /docs/gitexample/
---

{% highlight bash %}
git config --global user.name "Firstname LastName"
git config --global user.email "username@example.com"
git config -list

git clone <path to the git source, can be local path>
git pull <path to the git source, can be local path>


git diff
git diff --cached

git rm --cached readme.txt
git rm \*~
git rm log/\*.log
git mv file_from file_to

git log
git log -p -2
git log --stat
git log --pretty=format:"%h - %an, %ar : %s"
git log --pretty=format:"%h %s" --graph
git log --since=2.weeks
git log --pretty="%h - %s" --author=gitster --since="2008-10-01" \
                     --before="2008-11-01" --no-merges -- t/
git log --graph

git remote -v
git remote add pb git://github.com/paulboone/ticgit.git
git fetch pb
git remote show origin

git tag -a v1.4 -m 'my version 1.4'
git tag
git show v1.4
git tag v1.4-lw
git show v1.4-lw

git checkout -- <paths>
git branch testing
git checkout testing
git checkout master
git checkout -b iss53
git merge iss53
git branch -d iss53
git branch -v
git branch --merged
git branch --no-merged
git checkout -b serverfix origin/serverfix
git rebase master

git clone /opt/git/project.git
git remote add local_proj /opt/git/project.git
git pull /home/john/project
git clone --bare /path/to/git_project gitproject.git
git clone --bare my_project my_project.git
git init --bare --shared


{% endhighlight %}

