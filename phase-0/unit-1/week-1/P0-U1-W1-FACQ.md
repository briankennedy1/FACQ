#Week 1

##Command Line

####Q: What is a shell?
A: A shell is a program that allows you to interact with the computer. For shells that use the command line instead of graphics, you type in commands. So instead of clicking on a folder you can tell the computer to open it with a command e.g. cd documents. Shells have programs and those programs have commands.

####Q: What is a command line?
A: A command line allows a user to provide instructions and data to the operating system.

R: A digram of the command line: http://eglug.org/files/image_store/diagram2-454.png

####Q: What is a command?
A: "A command is provided by the client. Commands are usually one of three classes: 1. Internal - recognized and processed by the command line interpreter itself and not dependent upon any external executable file. (see what is a builtin?) 2. Included - A separate executable file generally considered part of the operating environment and always included with the OS.(see what is a utility?) 3. External executable files not part of the basic OS, but added by other parties for specific purposes and applications (see what is a utility?)"

####Q: What are parameters?
A: Parameters are either arguments or options. They generally follow commands on the command line and add details on what you want the command to do.

####Q: What are arguments?
A: Arguments are the values supplied to the command when it is called.

####Q: What are options?
A: An option modifies the action of a command and its result.

####Q: What's the difference between an option and an argument?
A: Imagine someone wants you to highlight the important parts of a chapter, and they want you to use a specific color, in this case pink. Well if this was a shell command we can think of highlight as the command, pink as the option, and chater 2 as the argument. From this analogy we see that options are  related to the process, and arguments are related to data. An actual example could be: cat < file1 > file 2, cat is the command, < & > are options related to the process, and file 1 & file 2 are arguments because they are related to the data.

####Q: What is a utility?
A: A utility is a program, more specifically it is a shell program. What does that mean? It means it is a piece of code that can be executed by the shell and does something very specific.

####Q: What is a builtin?
A: A shell builtin "is a command or a function, called from a shell, that is executed directly in the shell itself, instead of an external executable program which the shell would load and execute. Shell builtins work significantly faster than external programs, because there is no program loading overhead. However, their code is inherently present in the shell, and thus modifying or updating them requires modifications to the shell."

####Q: How can I tell if something is a builtin or a utility?
A: Type in man followed by the command and check under description or synposis. For example if you type in man cd,it says builtin under synopsis, and the description for man cat says cat says it is a utility.


####Q: What is a command prompt?
A: "A command prompt (or just prompt) is a sequence of (one or more) characters used in a command-line interface to indicate readiness to accept commands. Its intent is to literally prompt the user to take action. A prompt usually ends with one of the characters $, %, #, :, > and often includes other information, such as the path of the current working directory."

####Q:What are environmental variables?
A: They are names with values that affect they way a program runs on your computer. A running program can look at environmental variable values to determine what they should do with stuff. E.G. maybe a program wants to find out where to store something temporarily, they can look at your TEMP environmental variable to find out.