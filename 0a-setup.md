## Good practices

**Name your files well**

- Use lower case as much as possible.
- Do NOT use space.
- Do NOT use special characters expect for hyphen `-`.
    - underscore `_` is acceptable when you are not using SQL.
- Be concise. 
    - Bad: `excerpts-draft2-final1-approved.txt`
    - Better: `excerpts-2016-02.txt`
- Be descriptive.
    - Bad: `myfilefromclass-example02.html`
    - Better: `example-from-class.html`

**Tab completion**

It's very easy to typo commands, which can lead to errors and unintended consequences. One way of helping to avoid that problem is using tab completion, which allows the computer to finish typing a command that you have begun. Say you're in your home directory and want to go to the Desktop -- you'd type `cd Desktop`, right? You could also type `cd Des <tab>` and the computer would fill out the remaining text to spell "Desktop". This is a huge time-saver, especially when you're typing long directory paths (think something like `cd Desktop/projects/apps/django/test-app/test/apps/models.py`). [Here's a demo](http://www.youtube.com/watch?v=N8TaSgKJ-LM) of tab completion in action.

**Go straight home**

Your home directory is sort of like True North in command line world. It's a great way to orient yourself if you end up lost in the file system. In OSX, no matter where you are in the directory structure, you can immediately get back home by typing `cd`.

## Guides and cheat sheets

[Here's](http://wiseheartdesign.com/articles/2010/11/12/the-designers-guide-to-the-osx-command-prompt/) a useful guide for simple command line syntax on OSX and Linux. And [here's](http://www.bleepingcomputer.com/tutorials/windows-command-prompt-introduction/) another one for Windows.

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

_Kudos to [Sisi Wei](https://github.com/sisiwei/nyu-2015-spring-tutorials/blob/master/tutorials/command-line-basics.md) (who is a journalist at Propublica and will be teaching the Data Scraping class at CUNY-J in April) for synthesizing some of the materials._