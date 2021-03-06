# How to install cygwin (I'm kidding)

Like the bash sheet, I'm not going to differentiate between too much PS, the CLI, and common tools. It will become more apparent in the when scripting but for simple usage not so much

Basics

**[cmd] /?** - typing '/?' after a command will get you everywhere. It displays help info about a tool

**dir** - lists directory contents

**cd** - change directory

**cls** - clear screen

**mkdir** - make directory

**move** - move  a file from one path to another
 
**rename** - rename a file

**del** - delete a file

**rmdir** - delete a directory

## Commandlets

**Get-Process** - Gets the processes that are running on the local computer or a remote computer. Want something specific? Use the -name switch and separate the processes you're interested by comments

~~~
 Get-Process -Name firefox, powershell (I'll fix this later)
~~~

**Get-Alias** - Get-Alias takes an alias and returns the command name

~~~
PS /> Get-Alias

CommandType     Name
-----------     ----
…

Alias           cd -> Set-Location
Alias           cls -> Clear-Host
Alias           copy -> Copy-Item
Alias           dir -> Get-ChildItem
Alias           gc -> Get-Content
Alias           gmo -> Get-Module
Alias           ri -> Remove-Item
Alias           type -> Get-Content
...[Lotta Stuff here]
~~~

**Set-Location** - set the current working location to a specified path

~~~
PS /> Set-Location /home
PS /home>
~~~

**Get-ChildItem**

~~~
Get all files under the current directory:

PS /> Get-ChildItem

//Get all files under the current directory as well as its subdirectories:
PS /> cd $home
PS /home/jello> dir -Recurse

//List all files with "txt" file extension.

PS /> cd $home
PS /home/jello> dir –Path *.txt -Recurse

//Get-ChildItem -Path *.txt -Recurse -Force
~~~

**New-Item** Creates a new object. You can use the -Value parameter to add some data to your file. For example, the following command adds the phrase "Hello world!" as a file content to the test.txt. Because the (in this scenario) test.txt file exists already, we use -Force parameter to replace the existing content.
~~~
PS /home/jello> New-Item -Path ./test.txt -Value "Hello world!" -Force

    Directory: /home/jello


Mode                LastWriteTime         Length  Name
----                -------------         ------  ----
-a----         7/7/2016   7:19 PM             24  test.txt
~~~

**Set-Content**
~~~
PS /home/jello>Set-Content -Path ./test.txt -Value "Hello world again!"
~~~

**Get-Content**
Gets the content of the item at the specified location.
~~~
PS /home/jello> Get-Content -Path ./test.txt
PS /home/jello> type -Path ./test.txt
Hello world again!
~~~

**Remove-Item** - Deletes item

~~~
PS /home/jello> Remove-Item ./test.txt
~~~

**exit** Quit the PS game

## Powershell Scripting


---
Ref:https://github.com/PowerShell/PowerShell/tree/master/docs/learning-powershell
