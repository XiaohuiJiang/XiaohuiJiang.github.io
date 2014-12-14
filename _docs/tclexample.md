---
layout: docs
title: Tcl Examples
prev_section: gitexample
next_section: 
permalink: /docs/tclexample/
---

{% highlight tcl %}
# => rename some files with pattern 'prbs' by Tcl
set org_files [glob *prbs*]
foreach file $org_files { 
    puts $file; 
    regsub "prbs" $file "PRBS" fnew; 
    puts $fnew; 
    file rename $file $fnew;
}
{% endhighlight %}
