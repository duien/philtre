---
layout: post
title: Getting started with Semaphore
---

Getting up a well-integrated project is actually surprisingly easy.

Ingredients:

[Elixir Continuous Integration](https://semaphoreci.com/docs/elixir-continuous-integration.html)

[docs_ghpages](https://github.com/jjh42/docs_ghpages)

Make a few small changes to the project setup on Semaphore. You’ll need to add some git credentials to the setup, and then add a new post-build.

{% highlight sh %}
mix test
{% endhighlight %}

Tada! Now, whenever you push to master, you’ll autogenerate your hex docs and publish them to Github Pages.
