## What is a branch? Part 2

The [official git documentation](http://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging) is chill this time; it explains the concept with a fitting example in plain English, which you might find useful. 

![](http://cl.ly/image/1R292Y0h3K3Z/Screen%20Shot%202015-03-16%20at%203.59.22%20PM.png)

While you are not receiving calls for a hotfix yet (since you've been working on your own project, by yourself) sometimes you might like to table whatever mind-boggling css positioning you are working on at the moment, and switch to working on the Javascript you intend to use on that page.

For that purpose, this would be your workflow:

1. pause whatever you've worked on. At this moment, you've probably been only working on the `master`.
2. create a new branch and work on that one.
3. when you've done working on the new branch, merge it with with your main body of work, aka `master`.

![](https://farm3.staticflickr.com/2041/2211169294_e20eb51487.jpg)

_Remember me, the tree?_

![](http://www.bonsaiprimer.com/grafting/graftbranch.gif)

Merging is like taking a branch that has grown and graft it back to the main stem. Fortunately in git, it's not as gnarly as it is in bonsai.

## Practice

This is based in the js repo you've been using in this class:

1. From your current branch `master`, create a branch with `git checkout -b comment`
2. `You are on branch comment`. Good. Now add a comments in the js script.
3. Add, commit, push. You know the drill.
  - note that you push to the `word` branch with `git push origin comment`
4. `git checkout master`
5. `git merge comment` - Oh things are happening.
6. `git branch -d comment`

## Introducing the concept of production branch

Review a good workflow (hint: commit often.)

It matters to have a production branch. Say you've been working on your web page, and you decide to add a feature that takes you more than a few pushes. You would not want anyone who visit your page to see something broken or half-done. In this case, keep the public-facing work as it is, and branch off of that to continue working on your new thing.

The unbroken, steady version is your production branch. Question: **what is your production branch for your webpage?**

Next question: **keeping your production branch unchanged, what would you do if you would like to add some js experimentation to your page?**

## Homework

## Cheatsheet

http://rogerdudler.github.io/git-guide/
