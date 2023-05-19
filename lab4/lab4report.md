# Lab4report
## step4: Log into ieng6
<img width="818" alt="截屏2023-05-19 上午11 43 53" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/2edaf87a-7876-4198-98b4-342a5f1eb2d1">

```
#code use
#access to remore
ssh cs15lsp23ce@ieng6.ucsd.edu
ls
#delete used lab7 file
rm -rf lab7
#check deletion
ls
```

## step5: Clone your fork of the repository from your Github account
<img width="632" alt="截屏2023-05-19 上午11 44 08" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/daee5b30-bece-48b9-8d0a-b890a8de5f7d">

```
# git clone file from my repositry
git clone https://github.com/Jguan0330/lab7.git
#check clone
ls
```

## step6:Run the tests, demonstrating that they fail
<img width="698" alt="截屏2023-05-19 上午11 45 12" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/563ce748-97f7-444e-9ace-2540edcf71d0">

```
# enter lab7
cd lab7
#check current place
ls
# run the test
bash test.sh

```
## step7:Edit the code file ListExamples.java to fix the failing test (as a reminder, the error in the code is just that index1 is used instead of index2 in the final loop in merge)
<img width="806" alt="截屏2023-05-19 下午2 17 31" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/e8d89198-0864-49b8-b6a3-3db55c837d01">


```
(cursor should be at top-left)
esc
43j
11l
r2
:wq
Enter

```

## step8:Run the tests, demonstrating that they now succeed
<img width="874" alt="截屏2023-05-19 下午2 16 27" src="https://github.com/Jguan0330/cse15l-lab-reports/assets/114201575/fd09b35e-522a-450c-84ab-6c1230ef41fa">

```
bash test.sh
```

## step9:Commit and push the resulting change to your Github account