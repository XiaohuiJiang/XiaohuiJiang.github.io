---
layout: news_item
title: commands to install jekyll on ubuntu
author: XiaohuiJiang
version: 0.1
categories: [git]
---

{% highlight bash %}
sudo apt-get install ruby-full
sudo apt-get install gem
sudo apt-get install g++
`#download nodejs from http://nodejs.org`
ls ~/Downloads/
cd /tmp
tar zxvf ~/Downloads/node-v0.10.33.tar.gz 
cd node-v0.10.33/
vim README.md 
./configure 
make
sudo make install
sudo gem install github-pages
{% endhighlight %}
