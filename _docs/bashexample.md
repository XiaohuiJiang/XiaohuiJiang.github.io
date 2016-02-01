---
layout: docs
title: Bash Examples
prev_section: favorites
next_section: gitexample 
permalink: /docs/bashexample/
---

- [HowTo: Extract an RPM Package Files Without Installing It.](http://http://www.cyberciti.biz/tips/how-to-extract-an-rpm-package-without-installing-it.html) example:`rpm2cpio php-5.1.4-1.esp1.x86_64.rpm | cpio -idmv`
- send message to other terminals on the same machine:`echo "test" | wall`
{% highlight bash %}
# =>  remove some kinds of files under dir and subdir
$ find dir -name '*.[oa]' -print | xargs rm -f

# =>  copy or rename some files with pattern 'prbs'
$ ls *prbs* | sed  -n -r 's/(.*)prbs(.*)/cp & \1PRBS\2/ p' | sh
$ ls *prbs* | sed  -n -r 's/(.*)prbs(.*)/mv & \1PRBS\2/ p' | sh
$ find ./ -name '*PRBS*' -print | sed  -n -r 's/(.*)PRBS(.*)/mv & \1prbs\2/ p' | sh

# => sort and unique some lines and fields in a file
$ awk 'BEGIN { FS = ":" } ; {print $1, $3}' ./ts_changes.txt | sort -u
# => similar command can be used in VIM, also can change sequence of field
:105,112 !awk 'BEGIN { FS = ":" } ; {print $3, $1}' | sort -u
{% endhighlight %}

{% highlight bash %}
{% include code/bash_for.sh %}
{% endhighlight %}
- cscope info
{% highlight bash %}
{% include code/cscope.example %}
{% endhighlight %}


