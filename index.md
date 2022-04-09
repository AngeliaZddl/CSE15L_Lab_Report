## CSE15L Tutorial

_By Angelia_

Hello everyone, let's get starting with CSE15L today!

***
**Part 1 Install Visual Studio Code**

* Go to [Visual Studio Code website](https://code.visualstudio.com).
* Follow the instruction to download and install the application on your labtop.
* **important:** There are versions for all the major operating systems, like OSX (for Macs) and Windows (for PCs). Please make sure the version you download matching your computer.
* After installing, you should be able to open te window like this(there might be a little different on its appearance, dipending on your system and setting.)

![alt](VSCode.png)

**Part 2 Connect to a Remote Host**

* Follow the instruction [How-to-Reset-your-Password.pdf](How-to-Reset-your-Password.pdf) to activate your CSE15L server account.
* For windows users, `install OpenSSH` on your computer before starting.
* Then start to connect to a remote host:
1. Open a terminal in VSCode.
2. Do the command like this:

 `$ ssh cs15lsp22app@ieng6.ucsd.edu`
replace "app" with your special-course account.

3. You will probably recieve a message like this:

`⤇ ssh cs15lsp22app@ieng6.ucsd.edu`

`The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.`

`RSA key fingerprint is` 
`SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.`

`Are you sure you want to continue connecting (yes/no/[fingerprint])?`

Type yes and press enter.

4. Put in your password as required. You will have a view like this:
![alt](LogIn.png)

**Part 3 Run Some Commands**

Now you are connecting with the remote host if you have finished every step. 

Let's _try_ some commands:

* `$ cd` (change direction)
* `$ ls -lat` (list all files)
![alt](ls-lat.png)
* `$ ls <directory>` where `<directory>` is `/home/linux/ieng6/cs15lsp22/cs15lsp22abc`, where the abc is one of the other group members’ username.
![alt](ls-other.png)
* `$ cp` (copy)
![alt](Command_cp.png)
* `$ cat` (create or view a file)
![alt](Command_cat.png)
* Ctrl+D (exit)

**Part 4 Moving Files Over SSH with `scp`**
* Create a file called `WhereAmI.java` on your computer.
Content:

`class WhereAmI {
  public static void main(String[] args) {
    System.out.println(System.getProperty("os.name"));
    System.out.println(System.getProperty("user.name"));
    System.out.println(System.getProperty("user.home"));
    System.out.println(System.getProperty("user.dir"));
  }
}`


