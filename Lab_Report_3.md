# CSE15L_Lab_Report3

## Group Choice 1 – Streamline ssh Configuration

### `.ssh/config` and `ssh` command.

**I changed the name(after Host) to `Angelia` and then I can use `ssh Angelia` to log in the remote server.**

![Choice1](ChangeHostName.png)

## `scp` Command

**Now I can use some command with the name I set.**

![scp](Angelia_scp.png)
![ls](Angelia_ls.png)

***You may change that name to whatever you like!***

## Group Choice 2 – Setup Github Access from ieng6

### Public Key
**Here's the ssh stored on Github**
![github](github_ssh.png)

**Matching the key in my account**
![ieng6](account_ssh.png)

### Private Key
**This is the private token created and copied from Github. I stord it on the remote server by `git config --global credential.helper store`.**
![privatekey](git_privatekey.png)

### Running `git` Command While Logging Into ieng6 Account
![commit_and_push](commit_push_ssh.png)

### Link for the Resulting Commit
[CSE15L_Skill_Demo5](https://github.com/AngeliaZddl/CSE15L_Skill_Demo5/)

***Now it's no needs to put in the password every time while committing and pushing.***

## Group Choice 3 – Copy Whole Directories with `scp -r`

### Copying your whole markdown-parse directory

![scp_-r](spc_-r_markdown_parser.png)

### Logging into your ieng6 account after doing this and compiling and running the tests for your repository

**I made some changes for this file, deleting the .png files and then commit and push the changes to the origin main.**
![MarkdownParse1](Markdown_ieng6.png)
![MarkdownParse2](MarkdownParse_lib.png)
![MarkdownParse3](MarkdownParse_run_ieng6.png)

### Combining `scp`, `;`, and `ssh`: copy the whole directory and run the tests in one line

[Back to Main](https://angeliazddl.github.io/CSE15L_Lab_Report/)