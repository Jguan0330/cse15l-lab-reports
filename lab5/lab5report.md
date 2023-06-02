# Lab5report

## Part 1

1. student question

What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?

MAC, java, VScode

Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.

Here is the screenshoot of my code:
<br><img width="1728" alt="截屏2023-06-02 上午11 45 25" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/b878aef6-c654-4867-a478-2393fda0ba6a">
I expected to see no error message and the the task can pass, but the error message shows no junit find

Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.

this is the error message, and the code is from week6,I run 'bash grader.sh <URLs>'. My choose URL is correct and expects this to get full or near-to-full credit.
error message: 'package org.junit does not exist'
<br><img width="932" alt="截屏2023-06-02 上午11 45 35" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/1447328f-efd4-4840-86ec-324d62cc57d6">

2.TA's response
  
I see your code and the error message; think about your current direction; what might be some reasons that Junit does not exist in your current direction? As you can see, the provided file of JUnit is at lib. If you have any question free to ask!

3.Studetent's response
  
Yes, my current direction is at grading-area, I have go through the files in grading-area and I cannot find lib which stores Junit file, so I cp the lib into grading-area This solution works.
here is the file in grading-area before:
<br><img width="329" alt="截屏2023-06-02 下午2 20 41" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/ce50f51d-44c4-4aae-8de4-7eecdf41d04f">
  
<br>after solution:
<br><img width="329" alt="截屏2023-06-02 下午2 21 09" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/c97f947f-f4f5-48a9-bd33-553bedaf6214">
The correct version of code and result:
<br><img width="1728" alt="截屏2023-06-02 上午11 57 02" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/ffa4e78c-210c-4b73-a6a5-790d1311e0c2">
