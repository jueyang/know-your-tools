# Why command line

_Those familiar with working in the command line, however, wouldn’t trade its power, speed, and flexibility for anything, no matter how shiny or “user friendly” an alternative drag-and-drop interface might be._ - [Working with CSVs on the Command Line](http://bconnelly.net/working-with-csvs-on-the-command-line/)

### Let's take a step back

It's about workflow & the tools associated with it.

- find data
- get data
- clean data
- process data
- "analyze" data
- publish interpretations of data

### What we are doing today

- find data
- get data
- **clean data**
- **process data**
- **"analyze" data**
- publish interpretations of data

### This class will not teach you everything, but

_You're smart enough to look up more detail elsewhere once you know the idea or command to Google._ - [The Art of Command Line](https://github.com/jlevy/the-art-of-command-line/blob/master/README.md#meta)

# What is a command

Give me an example from Terminus, the game you played.

### Some of the commands we are using date way back

![](https://upload.wikimedia.org/wikipedia/commons/7/77/Unix_history-simple.svg)
- https://en.wikipedia.org/wiki/History_of_Unix

### Commands you might find useful

#### What's up

- `man`: manual
- `pwd`: print working directory
- `ls`: list items

#### Moving around

- `cd`: change directory
- `mkdir`: create new directory
- `touch`: create new file
- `rm`: remove
- `mv`: move or rename

#### Getting something from the internet

- `curl`: transfer a URL

#### Looking into data

- `cat`: print or concatenate
- `head`: first few rows of a file
- `tail`: last few rows of a file
- `wc`: word count (line count with `wc -l`*)

*= If you `man` one of these command, you will see that each command comes with many options. The dash and letter following a command is often referred to as a _flag_.

#### Searching and sorting

- `grep`: globally search a regular expression and print
  - `grep -i "SomeThing"` case insensitive
  - `grep -iw "something"` case insensitive, no substring
  - `grep -v "something"` give me anything BUT "something"
  - [many other useful flags](http://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/)
- `sort`
  - `sort -r file.txt`

#### Processing, I/O (input/output)

keywords: input, output, file, disk, user

- `>`: write output from a command to a file on disk*
- `>>`: append output from a command to an existing file on disk
- `|`: pass the output of one command to another for further processing 
- `<`: read a command's input from a disk file, rather than the user

*= If the file already exists, it will be overwritten.

# Must-knows

## Keep yourself sane

- Tab completion. `cat very-comlicated-name-really-01-just-kidding.txt.second.backup`
- Up arrow to go through your command history.
- Quit a shell console. Say you `man grep`, how do you get out? Type `q`.

## Good practices

- Back up. `cp original.file > original.file.backup`
- Name files wisely, by its content. **No space. No caps. No underscore.** `cat this-IS-A\ bad_file_name.txt > names-2014.txt`

# Further readings

- [Work with CSV on the Command Line](http://bconnelly.net/working-with-csvs-on-the-command-line/)
- A similar version of this class has been taught at NICAR15 and ONA15. See a more complete reading/tool list and credits in [this repo](https://github.com/chrislkeller/nicar15-command-line-basics).