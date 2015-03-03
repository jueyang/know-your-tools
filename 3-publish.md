## Publish your site on GitHub

So you got your site on `master`? Great, now we are going to use GitHub to host your site. To do this, you create a `gh-pages` branch. 

## What is a branch?

Ah. The talk of trees and branches. 

![](https://farm3.staticflickr.com/2041/2211169294_e20eb51487.jpg)

(It's still winter, so let's just stay on one branch right now. When the spring comes we'll be talking about more branches!)

## Publish

1. `git checkout -b gh-pages` Or if you feel like doing it step by step, you can do this in two steps, equivalent to this one:
  - `git branch gh-pages`
  - `git checkout gh-pages`
2. `git push origin gh-pages`

## View your site

`username.github.io/reponame`