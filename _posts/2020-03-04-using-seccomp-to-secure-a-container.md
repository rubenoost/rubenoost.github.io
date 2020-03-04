---
layout: post
title:  "Using seccomp to secure a container"
date:   2020-03-04 19:39:21 +0100
categories: jekyll docker security
---

Some code:

{% highlight c# %}
public void Assert(Func<bool> assertion)
{
    try
    {
        ValueIndexProvider = _searchSpace.GetValueIndexFor;

        while (!_searchSpace.IsExhausted)
        {
            if (assertion())
            {
                _searchSpace.CommitSuccess();
            }
            else
            {
                _searchSpace.CommitFailure();
            }
        }

        _searchSpace.ResolveAmbs();
        _searchSpace.ClearSuccesses();
    }
    finally
    {
        ValueIndexProvider = null;
    }
}
{% endhighlight %}