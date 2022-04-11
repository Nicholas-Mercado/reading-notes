# The Command Line Tasks

## The Command Line

I understood that I could add -something to a command to effect behavior but I didn't know there were called options

The first command line argument is a option and it is usually followed by a (-). Options can be used to modify a commands behavior.

bash - stands for Bourne again shell

## Basic Navigation

pwd which stands for Print Working Directory.

It was nice to get a explanation for that was returned with -l

-l stand for long list

- First character indicates whether it is a normal file ( - ) or directory ( d )
- Next 9 characters are permissions for the file or directory
- The next field is the group the file or directory belongs to (users in this case).
- Following this is the file size.
- Next up is the file modification time.
- Finally we have the actual name of the file or directory.
  
<cite>Basic Navigation! , <https://ryanstutorials.net/linuxtutorial/navigation.php></cite>

### Absolute and Relative Paths

Playing with and understanding the difference between relative vs absolute really helped stream line my navigation speed

Relative path - A file or directory location relative to where we currently are in the file system.

Absolute path - A file or directory location in relation to the root of the file system.

~ (tilde) - This is a shortcut for your home directory.

<cite>More About Files! , <https://ryanstutorials.net/linuxtutorial/aboutfiles.php></cite>

## More About Files

The following are some interesting facts about linux I did not know

Everything in linux is actually a file

file [path] - obtain information about what type of file a file or directory is.

Linux is case sensitive

## Manual Pages

The man command has already been useful when trying to figure out what and how I can use options

man [command] - Look up the manual page for a particular command.

Long hand command line options begin with two dashes

Short hand options begin with a single dash

## File Manipulation

Honestly I usually use vscode to to remove and move files but it is nice to know how to do it in Terminal

rmdir - remove/delete directory 

- -r -option allows you to remove directories that have files

mv[source][destination] - allows you to move and rename files

