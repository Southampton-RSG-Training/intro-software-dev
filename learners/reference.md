---
title: 'Reference'
---

# Bash Shell

## Other Resources and Further Learning

*   [Bash command reference](https://southampton-rsg.github.io/shell-novice/reference/index.html)
*   [Writing readable source code - a guide](https://software.ac.uk/resources/guides/writing-readable-source-code)
*   [Bash tutorial with online exercises](https://learnshell.org/)
*   [Intermediate guide to Bash](https://www.linode.com/docs/guides/an-intermediate-guide-to-bash-scripting/)
*   [Bash command cheat sheet](https://hackr.io/blog/linux-cheat-sheet)


## Glossary

[absolute path]{#absolute-path}
:   A [path](#path) that refers to a particular location in a file system.
    Absolute paths are usually written with respect to the file system's
    [root directory](#root-directory),
    and begin with either "/" (on Unix) or "\\" (on Microsoft Windows).
    See also: [relative path](#relative-path).
 
[argument]{#argument}
:   A value given to a function or program when it runs.
    The term is often used interchangeably (and inconsistently) with [parameter](#parameter).
 
[command shell]{#command-shell}
:   See [shell](#shell)
 
[command-line interface]{#command-line-interface}
:   An interface based on typing commands,
    usually at a [REPL](#read-evaluate-print-loop).
    See also: [graphical user interface](#graphical-user-interface).
 
[comment]{#comment}
:   A remark in a program that is intended to help human readers understand what is going on,
    but is ignored by the computer.
    Comments in Python, R, and the Unix shell start with a `#` character and run to the end of the line;
    comments in SQL start with `--`,
    and other languages have other conventions.
 
 
[current working directory]{#current-working-directory}
:   The directory that [relative paths](#relative-path) are calculated from;
    equivalently,
    the place where files referenced by name only are searched for.
    Every [process](#process) has a current working directory.
    The current working directory is usually referred to using the shorthand notation `.` (pronounced "dot").
 
[file system]{#file-system}
:   A set of files, directories, and I/O devices (such as keyboards and screens).
    A file system may be spread across many physical devices,
    or many file systems may be stored on a single physical device;
    the [operating system](#operating-system) manages access.
 
[filename extension]{#filename-extension}
:   The portion of a file's name that comes after the final "." character.
    By convention this identifies the file's type:
    `.txt` means "text file", `.png` means "Portable Network Graphics file",
    and so on. These conventions are not enforced by most operating systems:
    it is perfectly possible to name an MP3 sound file `homepage.html`.
    Since many applications use filename extensions to identify the [MIME type](#mime-type) of the file,
    misnaming files may cause those applications to fail.
 
[filter]{#filter}
:   A program that transforms a stream of data.
    Many Unix command-line tools are written as filters:
    they read data from [standard input](#standard-input),
    process it, and write the result to [standard output](#standard-output).
 
[flag]{#flag}
:   A terse way to specify an option or setting to a command-line program.
    By convention Unix applications use a dash followed by a single letter,
    such as `-v`, or two dashes followed by a word, such as `--verbose`,
    while DOS applications use a slash, such as `/V`.
    Depending on the application, a flag may be followed by a single argument, as in `-o /tmp/output.txt`.
 
[for loop]{#for-loop}
:   A loop that is executed once for each value in some kind of set, list, or range.
    See also: [while loop](#while-loop).
 
[graphical user interface]{#graphical-user-interface}
:   A graphical user interface,
    usually controlled by using a mouse.
    See also: [command-line interface](#command-line-interface).
 
[home directory]{#home-directory}
:   The default directory associated with an account on a computer system.
    By convention, all of a user's files are stored in or below her home directory.
 
[loop]{#loop}
:   A set of instructions to be executed multiple times. Consists of a [loop body](#loop-body) and (usually) a
    condition for exiting the loop. See also [for loop](#for-loop) and [while loop](#while-loop).
 
[loop body]{#loop-body}
:   The set of statements or commands that are repeated inside a [for loop](#for-loop)
    or [while loop](#while-loop).
 
[MIME type]{#mime-type}
:   MIME (Multi-Purpose Internet Mail Extensions) types describe different file types for exchange on the Internet,
    for example images, audio, and documents.
 
[operating system]{#operating-system}
:   Software that manages interactions between users, hardware, and software [processes](#process). Common
    examples are Linux, OS X, and Windows.
 
[orthogonal]{#orthogonal}
:   To have meanings or behaviors that are independent of each other.
    If a set of concepts or tools are orthogonal,
    they can be combined in any way.
 
[parameter]{#parameter}
:   A variable named in the function's declaration that is used to hold a value passed into the call.
    The term is often used interchangeably (and inconsistently) with [argument](#argument).
 
[parent directory]{#parent-directory}
:   The directory that "contains" the one in question.
    Every directory in a file system except the [root directory](#root-directory) has a parent.
    A directory's parent is usually referred to using the shorthand notation `..` (pronounced "dot dot").
 
[path]{#path}
:   A description that specifies the location of a file or directory within a [file system](#file-system).
    See also: [absolute path](#absolute-path), [relative path](#relative-path).
 
 
[pipe]{#pipe}
:   A connection from the output of one program to the input of another.
    When two or more programs are connected in this way, they are called a "pipeline".
 
[process]{#process}
:   A running instance of a program, containing code, variable values,
    open files and network connections, and so on.
    Processes are the "actors" that the [operating system](#operating-system) manages;
    it typically runs each process for a few milliseconds at a time
    to give the impression that they are executing simultaneously.
 
 
[prompt]{#prompt}
:   A character or characters display by a [REPL](#read-evaluate-print-loop) to show that
    it is waiting for its next command.
 
[quoting]{#quoting}
:   (in the shell):
    Using quotation marks of various kinds to prevent the shell from interpreting special characters.
    For example, to pass the string `*.txt` to a program,
    it is usually necessary to write it as `'*.txt'` (with single quotes)
    so that the shell will not try to expand the `*` wildcard.
 
[read-evaluate-print loop]{#read-evaluate-print-loop}
:   (REPL): A [command-line interface](#command-line-interface) that reads a command from the user,
    executes it, prints the result, and waits for another command.
 
[redirect]{#redirect}
:   To send a command's output to a file rather than to the screen or another command,
    or equivalently to read a command's input from a file.
 
[regular expression]{#regular-expression}
:   A pattern that specifies a set of character strings.
    REs are most often used to find sequences of characters in strings.
 
[relative path]{#relative-path}
:   A [path](#path) that specifies the location of a file or directory
    with respect to the [current working directory](#current-working-directory).
    Any path that does not begin with a separator character ("/" or "\\") is a relative path.
    See also: [absolute path](#absolute-path).
 
[root directory]{#root-directory}
:   The top-most directory in a [file system](#file-system).
    Its name is "/" on Unix (including Linux and Mac OS X) and "\\" on Microsoft Windows.
 
[shell]{#shell}
:   A [command-line interface](#command-line-interface) such as Bash (the Bourne-Again Shell)
    or the Microsoft Windows DOS shell
    that allows a user to interact with the [operating system](#operating-system).
 
[shell script]{#shell-script}
:   A set of [shell](#shell) commands stored in a file for re-use.
    A shell script is a program executed by the shell;
    the name "script" is used for historical reasons.
 
 
[standard input]{#standard-input}
:   A process's default input stream.
    In interactive command-line applications,
    it is typically connected to the keyboard;
    in a [pipe](#pipe),
    it receives data from the [standard output](#standard-output) of the preceding process.
 
 
[standard output]{#standard-output}
:   A process's default output stream.
    In interactive command-line applications,
    data sent to standard output is displayed on the screen;
    in a [pipe](#pipe),
    it is passed to the [standard input](#standard-input) of the next process.
 
 
[sub-directory]{#sub-directory}
:   A directory contained within another directory.
 
[tab completion]{#tab-completion}
:   A feature provided by many interactive systems in which
    pressing the Tab key triggers automatic completion of the current word or command.
 
[variable]{#variable}
:   A name in a program that is associated with a value or a collection of values.
 
[while loop]{#while-loop}
:   A loop that keeps executing as long as some condition is true.
    See also: [for loop](#for-loop).
 
[wildcard]{#wildcard}
:   A character used in pattern matching.
    In the Unix shell,
    the wildcard `*` matches zero or more characters,
    so that `*.txt` matches all files whose names end in `.txt`


# Version Control with Git 

## Git Cheatsheets for Quick Reference

- Printable Git cheatsheets in several languages are [available here](https://github.github.com/training-kit/) ([English version](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)). More material is available from the [GitHub training website](https://try.github.io/).
- An [interactive one-page visualisation](https://ndpsoftware.com/git-cheatsheet.html)
  about the relationships between workspace, staging area, local repository, upstream repository, and the commands associated with each (with explanations).
- Both resources are also available in other languages (e.g. Spanish, French, and more).
- "[Happy Git and GitHub for the useR](https://happygitwithr.com)" is an accessible, free online book by Jenny Bryan on how to setup and use Git and GitHub with specific references on the integration of Git with RStudio and working with Git in R.
- [Open Scientific Code using Git and GitHub](https://open-source-for-researchers.github.io/open-source-workshop/) - A collection of explanations and short practical exercises to help researchers learn more about version control and open source software.

## Glossary

[changeset]{#changeset}
:   A group of changes to one or more files that are or will be added
to a single [commit](#commit) in a [version control](#version-control)
[repository](#repository).

[commit]{#commit}
:   To record the current state of a set of files (a [changeset](#changeset))
in a [version control](#version-control) [repository](#repository). As a noun,
the result of committing, i.e. a recorded changeset in a repository.
If a commit contains changes to multiple files,
all of the changes are recorded together.

[conflict]{#conflict}
:   A change made by one user of a [version control system](#version-control)
that is incompatible with changes made by other users.
Helping users [resolve](#resolve) conflicts
is one of version control's major tasks.

[HTTP]{#http}
:   The Hypertext Transfer [Protocol](#protocol) used for sharing web pages and other data
on the World Wide Web.

[merge]{#merge}
:   (a repository): To reconcile two sets of changes to a
[repository](#repository).

[protocol]{#protocol}
:   A set of rules that define how one computer communicates with another.
Common protocols on the Internet include [HTTP](#http) and [SSH](#ssh).

[remote]{#remote}
:   (of a repository) A version control [repository](#repository) connected to another,
in such way that both can be kept in sync exchanging [commits](#commit).

[repository]{#repository}
:   A storage area where a [version control](#version-control) system
stores the full history of [commits](#commit) of a project and information
about who changed what, when.

[resolve]{#resolve}
:   To eliminate the [conflicts](#conflict) between two or more incompatible changes to a file or set of files
being managed by a [version control](#version-control) system.

[revision]{#revision}
:   A synonym for [commit](#commit).

[SHA-1]{#sha-1}
:   [SHA-1 hashes](https://en.wikipedia.org/wiki/SHA-1) is what Git uses to compute identifiers, including for commits.
To compute these, Git uses not only the actual change of a commit, but also its metadata (such as date, author,
message), including the identifiers of all commits of preceding changes. This makes Git commit IDs virtually unique.
I.e., the likelihood that two commits made independently, even of the same change, receive the same ID is exceedingly
small.

[SSH]{#ssh}
:   The Secure Shell [protocol](#protocol) used for secure communication between computers.

[timestamp]{#timestamp}
:   A record of when a particular event occurred.

[version control]{#version-control}
:   A tool for managing changes to a set of files.
Each set of changes creates a new [commit](#commit) of the files;
the version control system allows users to recover old commits reliably,
and helps manage conflicting changes made by different users.

# Python

## Glossary

[additive color model]{#additive-color-model}
:   A way to represent colors as the sum of contributions from primary colors
    such as [red, green, and blue](#rgb).

[argument]{#argument}
:   A value given to a function or program when it runs.
    The term is often used interchangeably (and inconsistently) with [parameter](#parameter).

[assertion]{#assertion}
:   An expression which is supposed to be true at a particular point in a program.
    Programmers typically put assertions in their code to check for errors;
    if the assertion fails (i.e., if the expression evaluates as false),
    the program halts and produces an error message.
    See also: [invariant](#invariant), [precondition](#precondition), [postcondition](#postcondition).

[assign]{#assign}
:   To give a value a name by associating a variable with it.

[body]{#body}
:   (of a function): the statements that are executed when a function runs.

[call stack]{#call-stack}
:   A data structure inside a running program that keeps track of active function calls.

[case-insensitive]{#case-insensitive}
:   Treating text as if upper and lower case characters of the same letter were the same.
    See also: [case-sensitive](#case-sensitive).

[case-sensitive]{#case-sensitive}
:   Treating text as if upper and lower case characters of the same letter are different.
    See also: [case-insensitive](#case-insensitive).

[comment]{#comment}
:   A remark in a program that is intended to help human readers understand what is going on,
    but is ignored by the computer.
    Comments in Python, R, and the Unix shell start with a `#` character and run to the end of the line;
    comments in SQL start with `--`,
    and other languages have other conventions.

[compose]{#compose}
:   To apply one function to the result of another, such as `f(g(x))`.

[conditional statement]{#conditional-statement}
:   A statement in a program that might or might not be executed
    depending on whether a test is true or false.

[comma-separated values]{#comma-separated-values}
:   (CSV) A common textual representation for tables
    in which the values in each row are separated by commas.

[default value]{#default-value}
:   A value to use for a [parameter](#parameter) if nothing is specified explicitly.

[defensive programming]{#defensive-programming}
:   The practice of writing programs that check their own operation to catch errors as early as possible.

[delimiter]{#delimiter}
:   A character or characters used to separate individual values,
    such as the commas between columns in a [CSV](#comma-separated-values) file.

[docstring]{#docstring}
:   Short for "documentation string",
    this refers to textual documentation embedded in Python programs.
    Unlike comments, docstrings are preserved in the running program
    and can be examined in interactive sessions.

[documentation]{#documentation}
:   Human-language text written to explain what software does,
    how it works, or how to use it.

[dotted notation]{#dotted-notation}
:   A two-part notation used in many programming languages
    in which `thing.component` refers to the `component` belonging to `thing`.

[empty string]{#empty-string}
:   A character string containing no characters,
    often thought of as the "zero" of text.

[encapsulation]{#encapsulation}
:   The practice of hiding something's implementation details
    so that the rest of a program can worry about *what* it does
    rather than *how* it does it.

[floating-point number]{#floating-point-number}
:   A number containing a fractional part and an exponent.
    See also: [integer](#integer).

[for loop]{#for-loop}
:   A loop that is executed once for each value in some kind of set, list, or range.
    See also: [while loop](#while-loop).

[function call]{#function-call}
:   A use of a function in another piece of software.

[immutable]{#immutable}
:   Unchangeable.
    The value of immutable data cannot be altered after it has been created.

[import]{#import}
:   To load a [library](#library) into a program.


[in-place operators]{#in-place-operators}
:   An operator such as `+=` that provides a shorthand notation for
    the common case in which the variable being assigned to
    is also an operand on the right hand side of the assignment.
    For example, the statement `x += 3` means the same thing as `x = x + 3`.

[index]{#index}
:   A subscript that specifies the location of a single value in a collection,
    such as a single pixel in an image.

[inner loop]{#inner-loop}
:   A loop that is inside another loop. See also: [outer loop](#outer-loop).

[integer]{#integer}
:   A whole number, such as -12343. See also: [floating-point number](#floating-point-number).

[invariant]{#invariant}
:   An expression whose value doesn't change during the execution of a program,
    typically used in an [assertion](#assertion).
    See also: [precondition](#precondition), [postcondition](#postcondition).

[library]{#library}
:   A family of code units (functions, classes, variables) that implement a set of
    related tasks.

[loop variable]{#loop-variable}
:   The variable that keeps track of the progress of the loop.

[member]{#member}
:   A variable contained within an [object](#object).

[method]{#method}
:   A function which is tied to a particular [object](#object).
    Each of an object's methods typically implements one of the things it can do,
    or one of the questions it can answer.

[object]{#object}
:   FIXME

[outer loop]{#outer-loop}
:   A loop that contains another loop.
    See also: [inner loop](#inner-loop).

[parameter]{#parameter}
:   A variable named in the function's declaration that is used to hold a value passed into the call.
    The term is often used interchangeably (and inconsistently) with [argument](#argument).

[pipe]{#pipe}
:   A connection from the output of one program to the input of another.
    When two or more programs are connected in this way, they are called a "pipeline".

[postcondition]{#postcondition}
:   A condition that a function (or other block of code) guarantees is true
    once it has finished running.
    Postconditions are often represented using [assertions](#assertion).

[precondition]{#precondition}
:   A condition that must be true in order for a function (or other block of code) to run correctly.


[regression]{#regression}
:   To re-introduce a bug that was once fixed.

[return statement]{#return-statement}
:   A statement that causes a function to stop executing and return a value to its caller immediately.


[RGB]{#rgb}
:   An [additive model](#additive-color-model)
    that represents colors as combinations of red, green, and blue.
    Each color's value is typically in the range 0..255
    (i.e., a one-byte integer).

[sequence]{#sequence}
:   FIXME

[shape]{#shape}
:   An array's dimensions, represented as a vector.
    For example, a 5&times;3 array's shape is `(5,3)`.

[silent failure]{#silent-failure}
:   Failing without producing any warning messages.
    Silent failures are hard to detect and debug.

[slice]{#slice}
:   A regular subsequence of a larger sequence,
    such as the first five elements or every second element.

[stack frame]{#stack-frame}
:   A data structure that provides storage for a function's local variables.
    Each time a function is called, a new stack frame is created
    and put on the top of the [call stack](#call-stack). When the function returns,
    the stack frame is discarded.

[standard input]{#standard-input}
:   A process's default input stream.
    In interactive command-line applications,
    it is typically connected to the keyboard; in a [pipe](#pipe),
    it receives data from the [standard output](#standard-output) of the preceding process.

[standard output]{#standard-output}
:   A process's default output stream.
    In interactive command-line applications,
    data sent to standard output is displayed on the screen;
    in a [pipe](#pipe),
    it is passed to the [standard input](#standard-input) of the next process.

[string]{#string}
:   Short for "character string",
    a [sequence](#sequence) of zero or more characters.

[syntax error]{#syntax-error}
:   CHECKME: a programming error that occurs when statements are in an order or contain characters
    not expected by the programming language

[test oracle]{#test-oracle}
:   A program, device, data set, or human being
    against which the results of a test can be compared.

[test-driven development]{#test-driven-development}
:   The practice of writing unit tests *before* writing the code they test.

[traceback]{#traceback}
:   CHECKME In Python, a list of the sequence of function calls that led to an error.

[tuple]{#tuple}
:   An [immutable](#immutable) [sequence](#sequence) of values.

[type]{#type}
:   CHECKME The classification of something in a program (for example, the contents of a variable)
    as a kind of number (e.g. [floating-point-number](#floating-point-number), [integer](#integer)), [string](#string), or something else.

[type of error]{#type-of-error}
:   CHECKME Indicates the nature of an error in a program, for example, `IOError` in Python refers to problems in input/output.
    See also [syntax error](#syntax-error).

[while loop]{#while-loop}
:   A loop that keeps executing as long as some condition is true.
    See also: [for loop](#for-loop).
