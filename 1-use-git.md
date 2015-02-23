## Website structure, git and GitHub

First, hope you had a good week navigating the command line. We will do a quick review, talk a bit about file structure, and dive into the git/GitHub workflow.

1. `cd` into your `snow` folder you created from last week 1. If you don't have a `snow` folder in your week 1 assignment, think why (consult the `i-did-it.png`).
2. Once you are in `snow`, type `pwd`.

File structure talk ensues. You can find the full text at the [end of document](https://gist.github.com/jueyang/740f4fd3d57ecfdbde39#more-on-file-strcuture).

## Git. On. It.

The internet is great. You find everything. For those of your who are wondering about the basics of git and GitHub, check out this piece of knowledge:

http://stackoverflow.com/questions/11816424/understanding-the-basics-of-git-and-github

In short, you are using `git` as a tool to track your changes, and `GitHub` as a service to 1) see these changes in a UI 2) collaborate with other people. Know that, yes, your building will be on the GitHub servers for now.

![](http://i.giphy.com/x4O0fjpQfoBZS.gif)

For an open project where no senstive information is involved, what GitHub offers, as infrastructure, is fab. Free space is not the main advantage we have here, because, y'know, there's something called digital storage that comes with your ID card here. Here's my for y'all in the room: who can tell me why we might favor **GitHub** over **digital storage**?

## Enough talk

Now let's put that ongoing construction of your building onto GitHub. In this session, we will "put a git on it."

**In GitHub:**

1. Create a repo.
2. Find the `https` clone, copy that.

**In Command Line:**

1. `cd` to the directory where `index.html` is.
2. `git init` -- Congrats! Now your content is version controled, just not on GitHub yet.
3. `git add -a`
4. `git commit -m 'first commit of the repo'`
5. `git remote add origin https://github.com/username/repo.git` -- Yes this is LONG. We'll deconstruct it in a sec!
6. check: `git remote -v`
7. `git push origin master` -- Congrats, wow! Now you can access your content from any computer, and other people can collaborate with you easily.

## Ok, time for homework of the week:

1. Add new things to your website. From now on you're making changes in GitHub for your site!
2. `git status` -- What do you see?
3. Let's follow the `add`, `commit`, and `push` workflow. It's similar to what you've done when you created the repo, but with a few modifications:

  1. `git add -p` -- Instead of `-a` which adds everything at once, and thus a bad practice, `-p` allows you to see what you've changed line by line, particularly useful once you know how painful debug can be with chunks of code/text. If you agree to all the change, press `y`. If you spot a typo or other error, press `q` to quit the adding process. Corrent that error, then do `git add -p` again.
  2. `git commit -m 'write something that explains your change, i.e. typo in article'`
  3. check: `git status`
  4. `git push origin master`

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

But as soon as you have other assets (photos, logos, videos, and later, if you dream big and you should, assortment of datasets) the one `index.html` file would no longer suffice -- or, if you will, sustain as the site grows. So one file breaks into pieces -- `css` gets its own folder, `js` its own. Your `html` might be modulized, etc. For larger newspapers, pretty crazy infrastructure has to happen (such as compling different sections of an html, to say the least) just to produce a page that you can make from ground up. Those processes will come later, and really depends on the organization involved (or if there's an organization at all.)

But for now, think of all the files you put in your site folder as a brick. Since what you are trying to accomplish is to complete the whole building [house emoji], getting to the right place where you can install a proper window frame is part of the building process.

**Too much metaphor? Here's the take-away:** Know the skeleton of your building. Follow the current construction convention (i.e. which folder goes where). Know where to look when adding a piece to the building. What happens when the building is finally done? It will be served somewhere. On the internet, how crazy. We'll talk about web servers in the future, but in case you are curious, check out this little snippet on [path translation](http://en.wikipedia.org/wiki/Web_server#Path_translation) (Indeed, you are learning how the internet works!)

