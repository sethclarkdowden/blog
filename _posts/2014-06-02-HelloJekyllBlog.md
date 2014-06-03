---
layout: post

title: Hello Jekyll
subtitle: "How I created this blog"
cover_image: tools.jpg

excerpt: "From zero to blog in 30min flat"

author:
  name: Seth Dowden
  twitter: Sethdowden
  gplus: 100687498195339762535 
  bio: the simple sage
  image: ks.png
---

>"Jekyll is a simple, blog-aware, static site generator perfect for personal, project, or organization sites."
[jekyll](https://github.com/jekyll/jekyll) was created by Tom Preston-Werner the co-founder of github. It works seamlessly with [github pages](https://pages.github.com/) making it quick and easy to start a blog or static website in minutes.

[incorporated](https://github.com/kippt/jekyll-incorporated) is a jekyll app that has a very clean style and is a greate base for creating your own jekyll blog.

{% highlight yaml %}
Terminal:
~ $ git clone https://github.com/kippt/jekyll-incorporated
~ $ cd jekyll-incorporated
~ $ bundle install
~ $ jekyll serve --watch
~ $ open http://localhost:4000/
{% endhighlight %}

Then make the blog your own by editing the  file and hacking around with the css to sute your prefrinces.

publishing your blog is as easy as creating a git repo  and adding the repo name to the Rakefile 

{% highlight yaml %} 
Rakefile:
# Change your GitHub reponame eg. "kippt/jekyll-incorporated"
GITHUB_REPONAME = "sethclarkdowden/Blog"
{% endhighlight %}

Then run

{% highlight yaml %}
Terminal:
~ $ rake site:publish
{% endhighlight %}

in a few minuts you will have your very own blog 