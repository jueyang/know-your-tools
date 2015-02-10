## Week 2: Website structure, git and GitHub

First, hope you had a good week navigating the command line. We will do a quick review, talk a bit about file structure, and dive into the git/GitHub workflow.

1. `cd` into your `snow` folder you created from last week. If you don't have a `snow` folder in your week 1 assignment, think why (consult the `i-did-it.png`).
2. Once you are in `snow`, type `pwd`.

File structure talk ensues. You can find the full text at the [end of document](https://github.com/jueyang/know-your-tools/blob/master/week2.md#more-on-file-strcuture).

## Git. On. It.

The internet is great. You find everything. For those of your who are wondering about the basics of git and GitHub, check out this piece of knowledge:

http://stackoverflow.com/questions/11816424/understanding-the-basics-of-git-and-github

In short, you are using `git` as a tool to track your changes, and `GitHub` as a service to:

1. see these changes in a UI, and 
2. collaborate with other people.

Know that, yes, your building will be on the GitHub servers (aka, _cloud_, which we will demystify over the course of this c lass) if you use it.

![](http://i.giphy.com/x4O0fjpQfoBZS.gif)

For an open project where no senstive information is involved, what GitHub offers, as infrastructure, is fab. Free space is not the main advantage we have here, because, y'know, there's something called digital storage that comes with your ID card here. 

**Here's my for question for y'all in the room:** who can tell me why we might favor **GitHub** over **digital storage**?

## Enough talk

Now let's put that ongoing construction of your building onto GitHub.

**In GitHub:**

1. Create a repo.
2. Find the `https` clone, copy that.

**In Command Line:**

1. `cd` to the directory where `index.html` is.
2. `git init` 
  - check 1: `ls -la` -- do you see a thing named `.git`? That's what the initialization did for you. Congrats! Now all your changes in the folder will be tracked by `git`, but none of it is on GitHub yet.
  - check 2: `git status` -- what do you see?
3. `git add -A` (note the captital `A`)
  - check: `git status` -- what do you see now?
4. `git commit -m 'first commit of the repository'` -- what does it say in the command line?
5. `git remote add origin https://github.com/username/repo.git` -- Yes this is LONG. We'll deconstruct it in a sec!
  - check: `git remote -v`
6. `git push origin master` -- Congrats! Now you can access your content from any computer, and other people can collaborate with you easily.

## Ok, time for homework of the week:

- First, add new things to your website. From now on you're making changes locally and pushing them to GitHub! This week's html assignment are the tags you add to your `index.html` (Check [the slide](http://mlouttit.com/cuny/lessons/w2/#/9/2) on your class website for deats.)
- After you're happy with your `index.html`, push the changes to GitHub. Remember the `add`, `commit`, and `push` workflow that you've done when you created the repo? We are going to do something very similar, just with a little modification. _Let's do this_:

1. check what changes you've made: can you tell me which command to use? Hint: see what we used many times to see files from being unstaged to staged.
2. `git add -p` -- Instead of `-A` which adds everything at once, and thus a bad practice, `-p` allows you to see what you've changed line by line, particularly useful once you know how painful debug can be with chunks of code/text. If you agree to all the changes, press `y`. If you spot a typo or other error, press `q` to quit the adding process. Correct that error, then do `git add -p` again.
  - check: yes, that command again.
2. `git commit -m 'write something that explains your change, i.e. typo in article'`
4. `git push origin master`

## Make life easier

There're a few git configuration you can do to make life easier. 

1.**More colors!** If you don't have colors in your iTerm, try this:
  ```
  git config --global color.ui true
  ```
2.**No more password-typing!** A world where you type the username and passwords only once is just so much better. To achieve that for your workflow:
  - Follow the steps [here](https://help.github.com/articles/set-up-git/#platform-mac)
  - Then [here](https://help.github.com/articles/caching-your-github-password-in-git/)
  - **Note:** the above are from the GitHub help pages. If you don't know what you are doing, it's totally fine. The important thing is that you **do** it. If you run into problems, send me a screenshot of your iTerm and [post an issue](https://github.com/jueyang/know-your-tools/issues). I'll help you out. 

---
## More on file strcuture

`path/to/your/file.thing`

```
  path
    - to
      - your
        - file.thing
```

```
  path
    - into the wilderness
    - to
      - airport
      - your
        - file.thing
        - rando
          - hi
```

### Why???

When you are constructing a web page, you might put all your code (html, css, js) in one file which you've learned to create: `index.html`.

But as soon as you have other assets (photos, logos, videos, and later, if you dream big and you should, assortment of datasets) the one `index.html` file would no longer suffice -- or, if you will, sustain as the site grows. So one file breaks into pieces -- `css` gets its own folder, `js` its own. Your `html` might be modulized, etc. For larger newspapers, pretty crazy infrastructure has to happen (such as compiling different sections of an html, to say the least) just to produce a page that you can make from ground up. Those processes will come later, and really depends on the organization involved (or if there's an organization at all.)

But for now, think of all the files you put in your site folder as a brick. Since what you are trying to accomplish is to complete the whole building [house emoji], getting to the right place where you can install a proper window frame is part of the building process.

**Too much metaphor? Here's the take-away:** Know the skeleton of your building. Follow the current construction convention (i.e. which folder goes where). Know where to look when adding a piece to the building. What happens when the building is finally done? It will be served somewhere. On the internet, how crazy. We'll talk about web servers in the future, but in case you are curious, check out this little snippet on [path translation](http://en.wikipedia.org/wiki/Web_server#Path_translation) (Indeed, you are learning how the internet works!)
