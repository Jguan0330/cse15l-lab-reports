# lab2report (week3)

## part1

I create a web server to have the function to store String values given by URL path and show the current and previous String values in the website.

<br><img width="765" alt="截屏2023-04-21 上午10 07 09" src="https://user-images.githubusercontent.com/114201575/233698106-3ad0516c-ce04-4e03-aff8-0677fb3cafa3.png">

<br>In the code, when a request is handled by the handleRequest method, the following methods are called:
1. url.getPath(): It is called to get the path of the given URI.
2. url.getQuery(): It is called to get the query part of the given URI.
3. String.split(): It is called to split the query into parameters based on the equal sign ("=").
4. ArrayList.add(): It is called to add a new message to the arr ArrayList.
5. String.join(): It is called to concatenate all the elements in the arr ArrayList with a newline separator ("\n").

<br>Relevant arguments to these methods and values of relevant fields:
* url: It is a URI object passed to the handleRequest method.
* arr: It is an ArrayList of strings used to store the messages. Its value will change as new messages are added.
* i: It is an integer variable used to store the number of messages in the arr ArrayList.
 
<br>How the values of relevant fields of the class change from this specific request:

* If the path of the URI contains "/add-message" and the parameter key is "s", the method adds the value of the "s" parameter to the arr ArrayList and increments the i variable by 1.
* If the conditions are not met (the path does not contain "/add-message" or the parameter key is not "s"), the arr ArrayList and the i variable remain unchanged.
* If the conditions are not met, the values don't change because the code doesn't execute the operations to add messages to the arr ArrayList and increment the i variable. Instead, it returns the "404 Not Found!" message.

<br>This is a example that I input {Junzheng Guan}, 
<br>The website alreadly store my previous values {Hello,jgua,fasdfadsf,ppap}:
<br><img width="489" alt="截屏2023-04-21 上午10 07 48" src="https://user-images.githubusercontent.com/114201575/233698137-bd7ebc07-c98a-4bc7-8fbe-d2cda1547fae.png">
<br>This is a example that I input {CSE15L LAB2} after I input {Junzheng Guan}.
<br>The website alreadly store my previous values {Hello,jgua,fasdfadsf,ppap}:
<br><img width="476" alt="截屏2023-04-21 上午10 08 05" src="https://user-images.githubusercontent.com/114201575/233698162-30d8c869-d876-4ef3-9e9a-367825b604fb.png">

## part2

```
#failed test
@Test
  public void testReversedore() {
    int[] input1 = {1,3,5,7};
    assertArrayEquals(new int[]{ 7,5,3,1}, ArrayExamples.reversed(input1));
  }
```

```
# not fail test
 @Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```

```
#original code
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
<br><img width="1320" alt="截屏2023-04-21 上午10 50 00" src="https://user-images.githubusercontent.com/114201575/233702277-f4ba80cb-cfab-47cb-a692-47a01c6d516f.png">

```
#fixed code
  static int[] reversed(int[] arr) {
    int[] newArray = new int [arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
<br><img width="1315" alt="截屏2023-04-21 上午10 50 58" src="https://user-images.githubusercontent.com/114201575/233702424-8d767e23-eff8-41cb-9d7c-0485a0501bf8.png">

## part3

