# CSE15L_Lab_Report4

The ***[link](https://github.com/AngeliaZddl/Lab7_markdown-parser)*** to markdown-parse repository

The ***[link](https://github.com/mv5903/markdown-parser)*** to the one reviewed in week 7

## Snippet 1

### Preview
![preview](snippet1.png)

### Test Code On My Own `markdown-parser`
![test11](test11.png)
### Test Code On The Lab7 Reviewed `markdown-parser`
![test12](test12.png)

### Running Result for On My Own `markdown-parser`
Not pass since the reason below:

![res11](result11.png)

### Running Result for The Lab7 Reviewed `markdown-parser`
Not pass since the reason below:

![res12](result12.png)

## Snippet 2

### Preview
![preview](snippet2.png)

### Test Code On My Own `markdown-parser`
![test21](test21.png)
### Test Code On The Lab7 Reviewed `markdown-parser`
![test22](test22.png)

### Running Result for On My Own `markdown-parser`
Not pass since the reason below:

![res21](result21.png)

### Running Result for The Lab7 Reviewed `markdown-parser`
Not pass since the reason below:

![res22](result22.png)

## Snippet 3

### Preview
![preview](snippet3.png)

### Test Code On My Own `markdown-parser`
![test31](test31.png)
### Test Code On The Lab7 Reviewed `markdown-parser`
![test32](test32.png)

### Running Result for On My Own `markdown-parser`
Not pass since the reason below:

![res31](result31.png)

### Running Result for The Lab7 Reviewed `markdown-parser`
Not pass since the reason below:

![res32](result32.png)

## Question 1:

*Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.*

### Answer: 
Yes, I would add if conditional sentence to check if the form of the link is correct. As the preview shows, if the link does not have a pair of `[` and `]` outside of a pair of the grave (`), then don't print the link.
For example, ![ex1](ex1.png) there is no close bracket before the grave symbol, so it is not a correct form for a link and then don't print it.

## Question 2:

*Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.*

### Answer:
Yes, I would add a for-loop and if conditional sentence to check if the content in a pair of bracket is a nested link. If a `(` is next to `(` or `)` and a `)` next to `)` or `(`, then it is a nested parenthesized link. If there is a pair of bracket with `\` inside of a pair of bracket, then it is escaped brackets

## Question 3:

*Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.*

### Answer: 
No, this case contains more than one tough exception. Firstly, I would add if conditional sentences to check `returns` inside a pair of brackets and parenthesis while the title of link is too long and take more than one line. Secondly, I would add for-loop and if conditional sentences to check if there's a close parenthesis.

## Explanation:



[Back To Main](https://angeliazddl.github.io/CSE15L_Lab_Report/)