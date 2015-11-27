# The mysterious invisible <CRLF>

How do we End a line and move to next line to be precise (Begining of the Next Line) ?

when you are using your computer to type something or The Computer displays one line after another line. The Computer should have some mechanism to mark the line ending.

So Should every editor, wordprocessor should do this ?

Yea, can be done but each and every editor will have a mechanism and worstly You can't open the same file in different editor. It would look akward. 

Hence, It should be done at the Operating System level and so that any editor can understand the line ending the same way and you would have great time working on the files.

## How do you do that?

Use a Character or a set of Character Code To mark the end of line. 

Lets go little closer and see. In a typewritter there are two operations that are done.

1. Carriage Return - in short CR - You push or return the Carriage to the begining of the position.

2. Paper Feed - Line Feed - You push the lever to bring the paper to next line. So that the Typewritter can type on blank space.

So MS-DOS, Windows Developers took this inspiration and implemented exactly the same way. They assigned Two Control Codes. One for Carriage Return and the other for Line Feed.

Hence MS-DOS, MS-Windows has CRLF character code for Newline / EndOfLine / LineBreak.

CR+LF is used in Windows '\r' 0x0D (in decimal 13) for CR and LF '\n' 0x0A (in decimal 10).

Creators of Unix are smarter enought to keep one single character code to do both the job of Carriage Return, Line Feed. LF is used in Unix.

## Can I see CRLF Characters ?

Yea, Lots of text editors have options to show invisible characters. You can enable those options and you can see in Notepad++ Editor.

![img]()





