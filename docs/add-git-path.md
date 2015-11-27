# Adding GIT PATH on Windows

## How do I add my GIT directory to the PATH on Windows?

### On Windows NT+ and Windows Server 2000+:

1.  Go to Control Panel and open the System icon (Start -> Settings -> Control Panel -> System, or just Start -> Control Panel -> System for Windows XP/2003+)
2. Go to the Advanced tab
3. Click on the 'Environment Variables' button
4. Look into the 'System Variables' pane
5. Find the Path entry (you may need to scroll to find it.
6. Double click on the Path entry
7. Enter your GIT directory at the end, including ';' before (e.g. ;C:\git
8. Press OK

### On Windows 98/Me you need to edit the autoexec.bat file:

Open the Notepad (Start -> Run and enter notepad)

1.  Open the C:\autoexec.bat file

2.  Locate the line with PATH=C:\WINDOWS;C:\WINDOWS\COMMAND;..... and add: ;C:\git to the end of the line

3.  Save the file and restart your computer

4.  Note: Be sure to reboot after following the steps above to ensure that the PATH changes are applied. 

## How do I add my GIT directory to the PATH On Mac

### Do the following

```
sudo vi /etc/paths
```

Add the git path in a line.



