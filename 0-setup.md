## Set up your computer

Here are the account, text editor and shell you will use for the class.

- [Register](https://github.com/) a GitHub account if you don't have one yet.
- Download [Sublime Text](http://www.sublimetext.com/).
- Download [iTerm2](http://iterm2.com/).

### Set up an environment for your tools

- Using spotlight (`command` + `space`), open iTerm2. 
- Install `homebrew`:
    - Paste the following into your iTerm window. Hit enter:

      ```
      ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
      ```

      _Say yes if it asks you to download xcode._

    - After that, make sure brew is configured correctly entering:

      ```
      brew doctor
      ```  

      _You might get some scary-looking messages, don't fret, we'll pause and take a look!_



### Install git

```  
brew install git
```

### Configure git

```
git config --global color.ui true
git config --global user.name "YOUR NAME"
git config --global user.email "YOUR@EMAIL.com"
```
Follow the instructions here to [cache GitHub password](https://help.github.com/articles/caching-your-github-password-in-git/) (so you don't have to enter it all the time).

### Set up habits

- Preferences > Keyboard.
  - fastest key repeat
  - shortest delay

- Create an alias so you can open files in Sublime Text from the Command Line.

```
ln -s '/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl' /usr/local/bin/subl
```

## Command Line Interface

**Q**: _How did we install and configure all the stuff above?_

**A**: Command Line.

In fact, before there was click/double click/drag, there was the Command Line. [Recommended reading](http://artlung.com/smorgasborg/C_R_Y_P_T_O_N_O_M_I_C_O_N.shtml).

- `cd` -- navigate to directory
- `ls` -- list all the content in the current directory
- `mkdir` -- make a directory within the current directory
- `touch` -- create a file within the current directory
- `mv` -- rename/move
- `rm` -- remove a file or directory within the current directory

Your new fam (in CLI):

- `.` -- you
- `..` -- mom
- `../..` -- granny

The many faces of `cd`:

- `cd Docouments` -- go to Documents
- `cd .` -- stay put
- `cd ..` -- go one level back (to mom's!)
- `cd ../..` -- go two levels back
- `cd` -- go back to the root directory

## Exercise

Consult the frequently used commands listed above.

1. Navigate to `Desktop`.
2. Create a new directory called `miceless`.
3. Navigate to `miceless`.
4. Create a new file called `name.txt`.
5. Open `name.txt` with `subl`.
    - What happens when you do `subl .`?
6. Add your name in the text file, save it.
7. Rename `name.txt` as `myname.txt`
8. Remove the text file.
9. Navigate back to `Desktop`.
10. Remove the directory `miceless`.
    - Use `rmdir` or `rm -r`.

## A little git primer

**What is it?**

`man git`

**Why are we using it?**

In short, you are using `git` to:

1. to track your changes

You are using [GitHub](https://github.com) as a service to:

1. see these changes in a UI, and 
2. collaborate with other people.

### Git of the week

Put a `git` on it.

In your website directory:

- `git init`
- `ls -a` -- What do you see?

Look around:

- `git status`

Find tips and cheatsheet in [this doc](https://github.com/jueyang/know-your-tools/blob/master/0a-setup.md).
