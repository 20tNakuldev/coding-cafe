1.What did `pwd` print?
    -> Using 'pwd' command showed me what is my file directory like for me it is showing = "\home\dell".
2.What did `ls -a` show that plain `ls` did not?
    -> "ls" command showed me only the folder name while "ls -a" command showed all the hidden files, including the file, "ls" command was showing in a particular directory where all these files are.
3.Pick one line from `ls -l`. What do you think the first column means?
    -> "drwxr-xr-x 4 dell dell 4096 Aug 25 04:38 coding-cafe" - This is what I can see After "ls -l" command, the letter d shows that right now i am at a directory while r,w and x shows that i have permissions to read , write and execute this file and then we have time, date and my system name and at last the name of my directory.
4.Why does that work from where you are standing? Which kind of path is coding-cafe/week02?Absolute or Relative?
    -> It works because the "coding-cafe" folder is located directly inside the current directory (the home folder). coding-cafe/week02 is a relative path because it does not start with a root slash (/) or a home symbol (~), meaning it navigates based on my current location.
5.mv did two different jobs above. What were they?
    -> The first mv command moved README-backup.md to week01 folder while the second mv command changed the name of README-backup.md to old-readme.md.
6.How many folders are on your PATH?
    -> On my PATH it is showing 25 folders.
7.Write down exactly where your python3 lives. You will need this again in a minute.
    -> My python lives in "/usr/bin/python3" according the command.
8.Compare your answer to 7 with the person next to you. Are they the same? If not, why might that be?
    ->My friend next to me have the same path for python3 that is "/usr/bin/python3" same as me.
9.What exactly did the shell say? Explain the error in your own words, using the word PATH.
    ->The shell returned 'Command not found' because it searched through every directory listed in my PATH variable. Since there was no file named pyton3 inside any of those folders, it could not run the command. And also it was trying to help me by asking that was I talking about 'python3'. (//Such a nice guy..) 
10..venv did not appear with plain ls. Why not?
    -> .venv did not appear with the first ls because files and folders that start with a dot (.) are hidden by default in Linux.
11.What changed about your prompt?
    -> The prompt changed by adding (.venv) to the very beginning. This acts as an indicator that the virtual environment is currently active.
12.Compare this with what you wrote down for question 7. Is it the same path? If not, what does that tell
you about what activate actually did to your PATH?
    -> No, it is not the same path; it now points to the Python inside the .venv folder instead of /usr/bin/python3. This tells me that the activate command temporarily modified my PATH variable, putting the virtual environment's folder at the very front so the shell finds it first.
13.What is in the second list that was not in the first?
    -> The second list contains requests along with its required dependencies (like charset-normalizer, idna, urllib3, requests and certifi), which were not present in the first list.
14.Where does python3 point now?
    ->The path points back to the system's global Python (at /usr/bin/python3) now that the virtual environment is turned off.
15.Find what ls -h does. Write it in your own words.
    ->The -h flag stands for 'human-readable'. It prints file sizes in a format like 1K, 234M, 2G instead of showing raw exact bytes.
16.What is the difference between what Ctrl + C and Ctrl + D did?
    ->Ctrl + C safely interrupts or cancels the current operation, but Ctrl + D sends an 'End of File' signal which completely closes the Python program and returns me to the terminal.