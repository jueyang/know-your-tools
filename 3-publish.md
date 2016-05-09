## Publish your site on GitHub

So you got your site on `master`? Great, now we are going to use GitHub to host your site. To do this, you create a `gh-pages` branch. 

## What is a branch?

Ah. The talk of trees and branches. 

![](https://farm3.staticflickr.com/2041/2211169294_e20eb51487.jpg)

(It's still winter, so let's just stay on one branch right now. When the spring comes we'll be talking about more branches!)

## Publish

There is also a branch specific to GitHub called `gh-pages`. If you push your website (with the appropriate html/css/js) under that branch you will be able to access the site via `USERNAME.github.io/REPONAME`.

- Make sure you name your html as `index.html`.
- Create a new branch called `gh-pages`.
  - `git checkout -b gh-pages`
- Check which branch you're on before you start working and before you push:
  - `git branch`
- Push to a remote (new) branch
  - `git push origin gh-pages`
