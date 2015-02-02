## Week 1: Get a GitHub account and get to know your computer (a bit more)

- [Register](https://github.com/) a GitHub account if you don't have one yet.
- Download these apps:
  - [Sublime Text](http://www.sublimetext.com/)
  - [iTerm2](http://iterm2.com/) (if you use a Mac)
- Set up your computer following the steps below. You only need to do these steps once per computer. Think of the steps as the first coat of seasoning of a cast iron -- pretty crucial before you starting cooking things with it. And, just like a cast iron, the more you use it, the better it gets:

  1. Install XCode via app store
  2. Open iTerm/teminal
  3. Install homebrew
    - Paste the following into your iTerm window. hit enter:
      `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
    - After that, make sure brew is configured correctly by running:
      `brew doctor` _you might some scary-looking messages, don't fret, we'll pause and take a look!_
  4. In iTerm/terminal, run the following commands:
    - `brew install git`
  
Alright, you are all set to use git and push content to GitHub. In the next class we'll try it out. 


### Opening the command line

Both Windows and OSX have built-in tools for accessing the command line.

On OSX, we are using iTerm2 instead of the built-in terminal. Click on the spotlight search on the topright of your screen, type "iTerm2" and open the CLI.

On Windows, navigate to the Start Menu and find the box called Run. Click on it. In the box that appears, type the letters cmd. This should open up your CLI.

## Ok, time for homework of the week:

You will find a list of frequently used commands in CLI at the bottom of this document. We'll practice four commands out of the list:

1. `cd` -- navigate to directory
2. `mkdir` -- make a directory within the current directory
3. `touch` -- create a file within the current directory
4. `rm` -- remove a file or directory within the current directory

In your DropBox folder for this week's assignment, do these:

1. Navigate to your DropBox folder with `cd`
2. Use `mkdir` to create a directory called `snow`
3. Navigate to the `snow` directory (hint: `cd`)
4. Use `touch` to create a file called `flake.txt`
5. Now, in your DropBox, you should see a file called `flake.txt` under the `snow` folder
6. Take a screenshot of your iTerm with all the commands, name it `i-did-it.png` and store it in your Dropbox folder
7. Now, in the CLI, use `rm` to remove the `flake.txt`
8. Is it gone? Check your Dropbox folder.

**If you run into problems for this assignment, please stop by Jue's desk this week. Make sure you've played around the commands before going to her. She can tell :p**

## Tips and tricks

Working with CLI can be difficult and tedious at first. Here are a few tips for making your command line lives a little easier:

**Tab completion**: It's very easy to typo commands, which can lead to errors and unintended consequences. One way of helping to avoid that problem is using tab completion, which allows the computer to finish typing a command that you have begun. Say you're in your home directory and want to go to the Desktop -- you'd type `cd Desktop`, right? You could also type `cd Des <tab>` and the computer would fill out the remaining text to spell "Desktop". This is a huge time-saver, especially when you're typing long directory paths (think something like `cd Desktop/projects/apps/django/test-app/test/apps/models.py`). [Here's a demo](http://www.youtube.com/watch?v=N8TaSgKJ-LM) of tab completion in action.

**Go straight home**: Your home directory is sort of like True North in command line world. It's a great way to orient yourself if you end up lost in the file system. In OSX, no matter where you are in the directory structure, you can immediately get back home by typing `cd`.

**Guides and cheat sheets**: [Here's](http://wiseheartdesign.com/articles/2010/11/12/the-designers-guide-to-the-osx-command-prompt/) a useful guide for simple command line syntax on OSX and Linux. And [here's](http://www.bleepingcomputer.com/tutorials/windows-command-prompt-introduction/) another one for Windows.

## List of common commands

### If you are using OSX:

<table>
    <tr>
        <th>Command</th>
        <th>Example</th>
        <th>What it does</th>
        <th>Notes</th>
    </tr>
    <tr>
        <td>pwd</td>
        <td>pwd</td>
        <td>Shows your present working directory</td>
        <td>Useful for keeping track of where you are</td>
    </tr>
    <tr>
        <td>ls</td>
        <td>ls</td>
        <td>Shows the contents of the current directory</td>
        <td>Can also use ls -a or ls -l to show more information about files</td>
    </tr>
    <tr>
        <td>cd</td>
        <td>cd Desktop</td>
        <td>Changes directories</td>
        <td>Use cd ..``` to move backwards</td>
    </tr>
    <tr>
        <td>mkdir</td>
        <td>mkdir new-directory</td>
        <td>Creates a new directory</td>
        <td></td>
    </tr>
    <tr>
        <td>touch</td>
        <td>touch test.py</td>
        <td>Creates a new file</td>
        <td></td>
    </tr>
    <tr>
        <td>mv</td>
        <td>mv test.py ./Desktop</td>
        <td>This isn't covered above, but mv moves or renames a file.</td>
        <td></td>
    </tr>
    <tr>
        <td>rm</td>
        <td>rm test.py</td>
        <td>Deletes a file</td>
        <td>Use with extreme caution. Once a file is deleted this way, you can't get it back.</td>
    </tr>
</table>

### If you are using Windows:

<table>
    <tr>
        <th>OSX command</th>
        <th>Windows equivalent</th>
    </tr>
    <tr>
        <td>pwd</td>
        <td>cd (with no arguments)</td>
    </tr>
    <tr>
        <td>ls</td>
        <td>dir or dir -p</td>
    </tr>
    <tr>
        <td>cd</td>
        <td>cd followed by the directory name (ex. cd Desktop)</td>
    </tr>
    <tr>
        <td>mkdir</td>
        <td>md</td>
    </tr>
    <tr>
        <td>touch</td>
        <td>None (sorry!)</td>
    </tr>
    <tr>
        <td>mv</td>
        <td>move</td>
    </tr>
    <tr>
        <td>rm</td>
        <td>del</td>
    </tr>
</table>

### Happy typing! Looking forward to seeing your vanished `snow/flake.txt` :)

![](http://media.giphy.com/media/7d00l0OLsunhm/giphy.gif)