# sed (Stream EDitor, a Unix utility) notes and recipes

***Sed editor***  

\*\*\* **Just append text to file**  

`sed -i '$a append_text' filename.txt  `
- _$ and a - must have options!!!_
- _$ - This address matches the last line of the last file of input, or the last line of each file when the -i or -s options are specified.
- _a - insert the text after matched pattern
 
 
 
*** **Find template and add new line after line with template**  

`sed -i '/search_text/a \\' filename.txt `
 
- _string - string to be found
- _-i - edit file in place
- _a - insert the text after matched pattern
- _\\ or \n - newline
 
 
*** **Find and replace text** 
 
`sed -i 's/found_text/replace_text/' filename.txt `


*** **Some more options** 
- _/t - tab character
