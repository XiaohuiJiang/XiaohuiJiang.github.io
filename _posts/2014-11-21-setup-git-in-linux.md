---
layout: news_item
title: set up git in ubuntu for github
author: XiaohuiJiang
version: 0.1
categories: [git]
---

for details please refer to https://help.github.com/articles/set-up-git/

{% highlight bash %}
sudo  apt-get install git
git --version

git config --global user.name "XiaohuiJiang"
git config --global user.email "XiaohuiJiang@users.noreply.github.com"
cat ~/.gitconfig 

sudo apt-get install curl
curl -s -O https://github-media-downloads.s3.amazonaws.com/osx/git-credential-osxkeychain
chmod u+x git-credential-osxkeychain
ls -l git-credential-osxkeychain 
sudo mv git-credential-osxkeychain "$(dirname $(which git))/git-credential-osxkeychain"

git config --global credential.helper osxkeychain
{% endhighlight %}
