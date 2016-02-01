![](https://media.giphy.com/media/JVtnyRL6XsI00/giphy.gif)

## Set up your computer

Here are the account, text editor and shell you will use for the class.

- [Register](https://github.com/) a GitHub account if you don't have one yet.
- Download [Sublime Text](http://www.sublimetext.com/).
- Download [iTerm2](http://iterm2.com/).

### Set up an environment for your tools

- Install Xcode via app store.
- Using spotlight (`command` + `space`), open iTerm2. 
- Install `homebrew`:
    - Paste the following into your iTerm window. Hit enter:

      ```
      ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
      ```

    - After that, make sure brew is configured correctly entering:

      ```
      brew doctor
      ```  

      _You might get some scary-looking messages, don't fret, we'll pause and take a look!_

### Set up git

- Install:

```  
brew install git
```

- Configure:

```
git config --global color.ui true
git config --global user.name "YOUR NAME"
git config --global user.email "YOUR@EMAIL.com"
```

### Set up habits

- Preferences > Keyboard.
  - fastest key repeat
  - shortest delay

- Create an alias so you can open files in Sublime Text from the Command Line.

```
ln -s '/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl' /usr/local/bin/subl
```

## Command Line Interface

Believe it or not, we've been using the CLI for a bit. How did we install and configure all the stuff above? 

Before there was click/double click/drag, there was the Command Line.

- `cd` -- navigate to directory
- `ls` -- list all the content in the current directory
- `mkdir` -- make a directory within the current directory
- `touch` -- create a file within the current directory
- `rm` -- remove a file or directory within the current directory

## Exercise

1. Create a directory in your `Documents` and name it `classes-spring-2016`.
2. Create a new file in the new directory and name it `spring.csv`.
3. `open` the `csv` file and start with the header for the csv
  - `name`, `day`, `prof`
  - eg. `html/css`, `Thu`, `Louttit/Yang`

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
