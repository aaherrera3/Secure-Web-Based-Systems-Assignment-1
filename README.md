# Secure-Web-Based-Systems-Assignment-1
Create a PHP program that produces exactly the same output as the provided java program.

Secure Web-Based Systems Fall 2020
CS 4339/5339 Professor L. Longpr´e
Assignment 1
You are given a java program that reads a file from a URL that contains
a program in a simple made-up programming language with no loops..
A grammar for the language is as follows:
* <input> ::= <section>*
* <section> ::= ’[’ <statement>* ’]’
* <statement> ::= <assignment> | <switch> | <output>
* <assignment> ::= ID ’=’ (INT | ID)
* <output> ::= ’output’ (INT | ID | STRING)
* <switch> ::= ’switch’ ID ’{’ <case>* [ ’default’ ’:’ <statement>* ] ’}’
* <case> ::= ’case’ INT ’:’ <statement>* ’break’
* ID ::= [a-zA-Z_]+
* INT ::= [0-9]+
* STRING starts and ends with double quotes ("), " can by escaped: (\")
The java program parses the input program and computes the result
for each section in the program. The program outputs an html page with
reformatted program sections and their result. When the program has syntax
errors, an error message for the first detected error is generated and the rest
of the section is skipped.
Create a PHP program that produces exactly the same output as the
provided java program. You need to compare the java program output to the
“page source” of the PHP program, not to what is displayed by the browser.
You do have to emulate exceptions caught by the java program. You do not
have to emulate exceptions that are not caught by the java program, like
errors in accessing the URLs. In your PHP program, use the PHP constant
PHP_EOL instead of \n for new lines. It should be more portable to different
implementation of PHP and operating systems. You can test your PHP
program by running it on your computer and comparing its output to the
output of the java program.
The instructor created a PHP program solution for this assignment. Although the instructor’s PHP program’s output was compared with the java
program’s output, there is always the possibility that the two programs are
not totally equivalent. If you find any discrepancies, please describe them to
the instructor. We will fix the PHP program solution.
To compare your program’s output against the instructor’s program output, unzip and place the 4 files included in the program testing .zip file provided and place them in the same folder, accessible from your localhost. In
the browser, navigate to that folder and bring up the page testPrograms.html.
Unless you’re on campus, you will need to VPN to UTEP for the comparison
program to access the instructor’s program.
Turn in:
Submit your program files and your report through blackboard.
In your report, include the answer to these questions:
1. Do you have any special instructions to the one who will test your
program? (If yes, explain.)
2. How long did you spend to do this assignment?
3. What problems (if any) did you encounter in this assignment, and if
yes, how did you solve the problems?
4. How effective was this assignment at helping you learning PHP?
5. Do you have any suggestion for a similar assignment next time we teach
this course?
Due date: Sunday, October 4, 11:59pm.