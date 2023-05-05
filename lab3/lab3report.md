# LAB3REPORT---Researching Commands for less
## 1.Show Line Numbers
Use the -N option to display the specified text file with line numbers. Displaying line numbers is useful for code reviews or paired programming because they make it easier to locate a specific issue.
```
less -N find-results.txt
```
[source](https://phoenixnap.com/kb/less-command-in-linux)
<br><img width="665" alt="截屏2023-05-05 下午12 09 26" src="https://user-images.githubusercontent.com/114201575/236548811-0c64d638-3df3-4044-aa2f-ca5154b8e913.png">
```
less -N grep-results.txt
```
[source](https://phoenixnap.com/kb/less-command-in-linux)
<br><img width="367" alt="截屏2023-05-05 下午12 18 02" src="https://user-images.githubusercontent.com/114201575/236550402-f6a1b976-adfe-4d96-9b89-22bcb820dc83.png">
## 2.Open File with Pattern Search
Use the -p option to open a text file on the page containing the first item that matches the specified pattern. The search is case-sensitive.
```
less -pbio find-results.txt
```
[source](https://phoenixnap.com/kb/less-command-in-linux)
<br><img width="539" alt="截屏2023-05-05 下午12 15 07" src="https://user-images.githubusercontent.com/114201575/236549996-042e68fa-4c68-4b6b-8b13-a8fde351287e.png">
```
less -preport find-results.txt
```
[source](https://phoenixnap.com/kb/less-command-in-linux)
<br><img width="604" alt="截屏2023-05-05 下午12 17 16" src="https://user-images.githubusercontent.com/114201575/236550206-7bf799fb-2527-4f4c-97af-8e4ba16b820a.png">

## 3.Remove Multiple Blank Lines
The -s option squeezes multiple blank lines from a text file into one blank line. Removing multiple blank lines allows less to show more content in each screenful of the file.
```
less -s technical/biomed/1468-6708-3-1.txt
```
<br><img width="1728" alt="截屏2023-05-05 下午12 35 48" src="https://user-images.githubusercontent.com/114201575/236553511-599fca65-8b2e-40b0-81d0-1cbc0ffc8b02.png">

```
less -s technical/911report/chapter-1.txt
```
<br><img width="1728" alt="截屏2023-05-05 下午12 39 28" src="https://user-images.githubusercontent.com/114201575/236554118-60e07de7-ab06-4c2d-8e68-9053b50893f2.png">

## 4.Keep Content on Screen After Quitting
After quitting less, the terminal window clears, removing the file output. To leave the file contents in the terminal after quitting, specify the -X option.
```
less -X find-results.txt
```
<br><img width="553" alt="截屏2023-05-05 下午2 34 56" src="https://user-images.githubusercontent.com/114201575/236572829-fdf771cd-5826-406d-8e59-0660d84ac4dd.png">


```
less -X technical/911report/chapter-1.txt
```
<br><img width="627" alt="截屏2023-05-05 下午2 35 30" src="https://user-images.githubusercontent.com/114201575/236572837-e9420fc5-0bc4-4bf3-86e5-e5432cf1c404.png">

