# webpack-for-scss  

***Sed editor***  

***Just append text to file*  

sed -i '$a append_text' filename.txt  
_$ and a - must have options!!!_  
 
 
 
***Find template and add new line after line with template*  

$ sed -i '/search_text/a \\' filename.txt 
 
string - string to be found 
_-i - edit file in place_ 
_a - insert the text after matched pattern_ 
_\\ or \n - newline _ 
 
 
***Find and replace text* 
 
$ sed -i 's/found_text/replace_text/' filename.txt 
