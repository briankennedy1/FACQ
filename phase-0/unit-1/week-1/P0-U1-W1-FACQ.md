#Command Line

####Q: What is a shell?
A: A shell is a program that allows you to interact with the computer. For shells that use the command line instead of graphics, you type in commands. So instead of clicking on a folder you can tell the computer to open it with a command e.g. cd documents. Shells have programs and those programs have commands.

####Q: What is a command line?
A: A command line allows a user to provide instructions and data to the operating system.

R: A digram of the command line: http://eglug.org/files/image_store/diagram2-454.png

####Q: What is a utility?
A: A utility is a program, more specifically it is a shell program. What does that mean? It means it is a piece of code that can be executed by the shell and does something very specific.

####Q: What is a builtin?
A: A shell builtin "is a command or a function, called from a shell, that is executed directly in the shell itself, instead of an external executable program which the shell would load and execute. Shell builtins work significantly faster than external programs, because there is no program loading overhead. However, their code is inherently present in the shell, and thus modifying or updating them requires modifications to the shell."

####Q: How can I tell if something is a builtin or a utility?
A: Type in man followed by the command and check under description or synposis. For example if you type in man cd,it says builtin under synopsis, and the description for man cat says cat says it is a utility.


