# _**VIVIN'S LAB REPORT 2:**_

# Code Change 1:
This change will aim to fix the error of having an image in the frist line after the title of the [test file](Test-file2.md). Essentially allowing the code to work on files with both links and images.
The symptom is shown below:
![Symptom1](imageerrorsymptom.png)
As seen the image name is also printing which shouldnt happen as this is only to print actual links and not image names.

The following code change was made: 
![Change 1](imagefix.png)

Finally as seen above we added an if statement to ensure 

```
 if(markdown.charAtnextOpenBracket-1)=='!') 
```
By doing so we check if the ! mark exists after the first '(' we know its an image and hence dont need this data and we use 'continue' to skip this line and go to the next. By doing so everytime we hit a '!' we dont record the image name and instead go to the next line to check for a link. 

# Code Change 2:




