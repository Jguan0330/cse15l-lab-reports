# lab1 report(week1)

CSE15L account tutorial

It is very important to find you CSE15L account! The following steps will teach you how to find your personal account.
* You can find your personal CSE15L account: [Link](https://sdacs.ucsd.edu/~icc/index.php)
* Please to reset password: [Link](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit)
* Here is a tutorial: [Link](https://drive.google.com/file/d/17IDZn8Qq7Q0RkYMxdiIR0o6HJ3B5YqSW/view)
* You need to wait 15mins to let reset finished :) 
# Be patient!!!
Many people usually fail in find the account because they cannot log into remote service. One tip is that your can test your account and your new password through LAB computer to ensure you already reset your account!

## 1. Installing VScode 
There is always first priority for code writer to have a good tool. VScode is lightweight and powerful and can be easily installed on any platform. VS Code has built-in support for Node. js, TypeScript, and JavaScript and a feature-rich extension ecosystem for different languages like C++, Java, C#, PHP, Go, and Python. Let's looks at how to install VScode
* vscode download: [Link](https://code.visualstudio.com/)
* If you took CSE11 Before, you can skip the vscode setup!
* I already finished installation during CSE11 so I skip this process.

<img width="1728" alt="截屏2023-04-05 下午5 14 00" src="https://user-images.githubusercontent.com/114201575/230249198-cd6c26f8-a149-4177-b0a6-81ac76d411a8.png">

## 2. Remotely Connecting
A terminal, also known as a command-line interface, provides several benefits over a graphical user interface (GUI). Firstly, it is more efficient as it allows for faster execution of commands and can perform a wide range of tasks, from simple file manipulation to complex scripting and automation. Secondly, it enables remote access to servers and computers, making it a convenient tool for system administrators. Additionally, terminals use fewer system resources than a GUI, making it a better choice for systems with limited resources. Furthermore, terminals provide a powerful environment for scripting and automation, simplifying and streamlining repetitive tasks. Finally, terminals can be customized to suit specific needs, extending their functionality.
* You can use this code to log in remote servior: 
```
# You can replace xx with personal code! e.g. cs15lsp23zz@ieng6.ucsd.edu 
ssh cs15lsp23xx@ieng6.ucsd.edu
```
* This message might appear on your computer if it is the first time you connect to this server.
```
# I recommand to select YES.
⤇ ssh cs15lwi23zz@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```
* You can enter you password(same as reset password)
* If successful there will be information appear/if not you need to enter password again or wait until password successfully reset
* hint: you can log in you account in lab computer username:/password: to sure your password already reset!
* Don't worry about failure log in, once you can successful log in account though lab computer, you just need to wait a few minutes

<img width="1728" alt="截屏2023-04-05 下午5 40 39" src="https://user-images.githubusercontent.com/114201575/230249206-870d5a8a-5790-438a-ac45-135f1f501410.png">

## 3. Trying Some Commands
We need to know how this remote terminal works. So here are some fundamental but essential commands you need will find useful!

* The **pwd** command writes to standard output the full path name of your current directory (from the root directory). All directories are separated by a / (slash). 

<img width="334" alt="截屏2023-04-19 下午4 10 07" src="https://user-images.githubusercontent.com/114201575/233219128-752f9315-01c8-4ae9-8c37-54daf914823e.png">

* The **ls** command is used to list files or directories in Linux and other Unix-based operating systems.

<img width="332" alt="截屏2023-04-19 下午4 10 30" src="https://user-images.githubusercontent.com/114201575/233219172-d4286638-2fe4-4a9c-abf6-d8d96288873e.png">

* The **cd** command, also known as chdir (change directory), is a command-line shell command used to change the current working directory in various operating systems.

<img width="945" alt="截屏2023-04-19 下午4 10 56" src="https://user-images.githubusercontent.com/114201575/233219253-34d6309d-aa27-4532-87f7-89c970c644f6.png">
  
* The **cp** command will create a copy of the contents of the file or directory specified by the SourceFile or SourceDirectory parameters into the file or directory specified by the TargetFile or TargetDirectory parameters.

<img width="949" alt="截屏2023-04-19 下午4 20 00" src="https://user-images.githubusercontent.com/114201575/233220084-edda4f62-9a9a-413d-b15a-b5f591d92bc1.png">

* The **cd ..** command will help you to go up one level of the directory tree. 

<img width="323" alt="截屏2023-04-19 下午4 20 08" src="https://user-images.githubusercontent.com/114201575/233220128-84008098-7bf5-4b6a-b8de-0c4345efadc7.png">
  
* The **cat** command reads each File parameter in sequence and writes it to standard output. If you do not specify a file name, the cat command reads from standard input.

<img width="330" alt="截屏2023-04-19 下午4 23 36" src="https://user-images.githubusercontent.com/114201575/233220363-7af37503-954a-469c-91de-9ee5abaa475e.png">
 
* The **exit** command is to disconnect the connection between your computer and remote servicor.

<img width="334" alt="截屏2023-04-19 下午4 25 53" src="https://user-images.githubusercontent.com/114201575/233220667-a6498b33-e189-4273-a9b5-1865a7bc0aaf.png">

* A series of commands like cd, ls, pwd, mkdir, and cp.

<img width="1728" alt="截屏2023-04-05 下午6 02 42" src="https://user-images.githubusercontent.com/114201575/230249210-97501740-7edb-46e2-a396-cf2f949f6bd9.png">

# END
