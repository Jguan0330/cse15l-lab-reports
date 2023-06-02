# Lab4report
## step4: Log into ieng6
<img width="818" alt="截屏2023-05-19 上午11 43 53" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/2edaf87a-7876-4198-98b4-342a5f1eb2d1">

```
#code use
#access to remore
ssh cs15lsp23ce@ieng6.ucsd.edu
<enter>
# log in to accout without typing password, see explain below
ls
<enter>
#delete used lab7 file
rm -rf lab7
<enter>
#check deletion
ls
<enter>
```
## explain of ssh key(copy from week7 page)
#link below https://ucsd-cse15l-s23.github.io/week/week7/
1. In your local terminal, run ssh-keygen
2. Keep entering <Enter> until the program shows some text it calles the “randomart image”.
Note the path where the public key is saved (underlined below).
<img width="517" alt="截屏2023-06-02 上午10 53 22" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/77b3b648-29ad-40e8-8236-9b80a42a2ecb">
3. Now, log into your remote course specific account on ieng6
4. Run mkdir .ssh in the terminal
5. Logout of your remote account
6. Now, we want to copy the public SSH key you created onto your remote account, specifically inside the .ssh directory you just created, in a file called authorized_keys.
7. Scroll up a bit to where you were creating the SSH key, find the line where it says: Your public key has been saved in: <path to your public SSH key>, copy the path. Make sure you get the public key file, ending in .pub, here, not the private file.
8. From your local computer, run scp <path to your public SSH key> cs15lsp23__@ieng6.ucsd.edu:~/.ssh/authorized_keys
Enter password when prompted (this will be the last time you have to type it!)
  
## step5: Clone your fork of the repository from your Github account
<img width="636" alt="截屏2023-05-19 下午2 47 56" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/bd35c3e4-2b2e-421a-9e15-4b94ef1bf99e">


```
# git clone file from my repositry
git clone git@github.com:Jguan0330/lab7.git
<enter>
#check clone
ls
<enter>
```

## step6:Run the tests, demonstrating that they fail
<img width="698" alt="截屏2023-05-19 上午11 45 12" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/563ce748-97f7-444e-9ace-2540edcf71d0">

```
# enter lab7
cd lab7
<enter>
#check current place
ls
<enter>
# run the test
bash test.sh
<enter>

```
## step7:Edit the code file ListExamples.java to fix the failing test (as a reminder, the error in the code is just that index1 is used instead of index2 in the final loop in merge)
<img width="806" alt="截屏2023-05-19 下午2 17 31" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/e8d89198-0864-49b8-b6a3-3db55c837d01">

```
(cursor should be at top-left)
#The Escape key is pressed to ensure the cursor 
#is not in any insert or command mode before starting the sequence. 
<esc> 
#The number 43 represents a count, and j moves 
#the cursor down one line. So, 43j moves the cursor down 43 lines.
43j   
#The number 11 is a count, and l moves the cursor 
#one character to the right. Therefore, 11l moves the cursor 11 characters to the right.
11l   
#The r command is used to replace the character under 
#the cursor with another character. So, the character under the cursor, which is 1, is replaced with 2.
#the cursor now point at 1
r2    
#The : puts Vim into command-line mode, and wq 
#is a shorthand for the write and quit commands. It saves the file and exits the editor.
:wq   
#Pressing the Enter key executes the command entered 
#in the previous step, which is :wq. It saves the changes and exits Vim.
<enter> 

```

## step8:Run the tests, demonstrating that they now succeed
<img width="874" alt="截屏2023-05-19 下午2 16 27" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/fd09b35e-522a-450c-84ab-6c1230ef41fa">

```
bash test.sh
<enter>
```

## step9:Commit and push the resulting change to your Github account
<img width="589" alt="截屏2023-05-19 下午3 24 15" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/0c51ae1e-840f-4206-90b5-a8dfb77f2336">

<img width="596" alt="截屏2023-05-19 下午3 24 02" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/dd039a17-4b85-42c2-82dd-6600609f84e8">

```
git commit --amend
<enter>
<Esc>
:wq
<enter>
git config --global pull.rebase true
<enter>
git pull git@github.com:Jguan0330/lab7.git main
<enter>
git push git@github.com:Jguan0330/lab7.git main
<enter>
```

