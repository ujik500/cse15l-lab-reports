# Week 4 Lab Report
## Code Change #1
The first failure-inducing input I noticed was a file with whitespace at the end, which caused MarkdownParse to enter an infinite loop. The file that caused this symptom was called test-file.md, and you can see that [TODO](). Here is an example of the symptom:

![Image2](week4pic2.PNG)

To fix this, I added some if statements that break out of the while loop if no more links are detected in the file (resulting in the indices being set to -1). The changes from this commit are displayed below:

![Image1](week4pic1.PNG)

## Code Change #2


## Code Change #3
