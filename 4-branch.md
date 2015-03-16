## What is a branch? Part 2

The [official git documentation](http://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging) is chill this time; it explains the concept with a fitting example in plain English, which you might find useful. 

![](http://cl.ly/image/1R292Y0h3K3Z/Screen%20Shot%202015-03-16%20at%203.59.22%20PM.png)

While you are not receiving calls for a hotfix yet (since you've been working on your own project, by yourself), sometimes you might like to table whatever mind-boggling css positioning you are working on at the moment, and switch to working on the Javascript you intend to use on that page.

For that purpose, this would be your workflow:

1. keep whatever you've worked on
2. start something on a new branch
3. when that new thing is ready on the new branch, incoporate it with with your main body of work

![](https://farm3.staticflickr.com/2041/2211169294_e20eb51487.jpg)

_Remember me, the tree?_

## Practice

This is based in the js repo you've been using in this class:

1. From your current branch `master`, create a branch with `git checkout -b comment`
2. `You are on branch comment`. Good. Now add a comments in the js script.
3. Add, commit, push. You know the drill.
  - note that you push to the `word` branch with `git push origin comment`
4. `git checkout master`
5. `git merge comment` - Oh things are happening.
6. `git branch -d comment`

## Homework

Create a `js` branch off your `gh-pages`. You will start fiddling with the Javascript for your webpage o

`git checkout -b js`
