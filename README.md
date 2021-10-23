# webpack-for-scss

***Sed editor***

***Find template and add new line after line with template

$ sed -i '/search_text/a \\' filename.txt

string - string to be found
-i - edit file in place
a - insert the text after matched pattern
\\ - newline 


***Find and replace text

$ sed -i 's/found_text/replace_text/' filename.txt
