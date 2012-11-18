# Stubber
Stubber consists of a commandline program 'Stubber' by Steven E.
Nameroff and a frontend by me.

Stubber creates stubs on the basis of a Ada specifikation given to it.
The stubs are placed in a Ada body file which will be written into a adb
directory in the specifikation files parent directory. The adb
directory is created if it does not exist already.

NOTE: This is a RISC OS app and will not work on other platforms.

## Frontend use

1. Double click on the !Stubber icon - this will place an icon on the iconbar.
2. SELECT clicking on the iconbar icon will open a setup window.
3. Fill in the information needed and SELECT click on 'Run'. Use the interactive help to get information about what to fill in where.

This will start the Stubber command line program and open a window
showing the status.

This program stubs anything in your program that needs to be stubbed. You need do nothing to tell the stubber what needs to be stubbed; it figures it out by itself. It is imperative that the program being stubbed is syntactically correct,  at least to the point that each 'if' has and 'end if', etc.  If this is not the case, then the stubber will self-destruct or worse than that, it will miss-stub your program. This stubber will also keep you informed as to where it is and what's being stubbed.

# Command line use
Stubber only takes one argument - the name & path of the Ada specification.