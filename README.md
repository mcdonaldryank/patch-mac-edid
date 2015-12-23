# patch-mac-edid
Fork of  to Gist from https://gist.github.com/adaugherity/7435890 that allows for fix with color and flickering when attaching a Mac to a remote monitor

##TO USE:
1. Boot your Mac into safe mode by pressing and holding ```CMD + R``` until the Apple logo appears during boot.
2. Once in safe mode, select terminal from the Utilities menu.
3. In the terminal typs ```csrutil disable```
4. Select the apple icon at the top right and select reboot.
5. Execute ```sudo ruby patch-edid.rb``` with monitor connected to your Mac.
6. Move the new directory that is created in the same directory as your script execution to ```/System/Library/Displays/Contents/Resources/Overrides/```
7. Reboot your machine with external monitor connected
8. Verify all is working.
9. Reboot machine back into safe mode following same steps as 1 and 2 above.
10. Using the terminal in safe mode type ```csrutil enable```, follow step 4 and enjoy. 
