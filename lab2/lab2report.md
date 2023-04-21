# lab2report (week3)

## part1

I create a web server to have the function to store String values given by URL path and show the current and previous String values in the website.
<img width="765" alt="截屏2023-04-21 上午10 07 09" src="https://user-images.githubusercontent.com/114201575/233698106-3ad0516c-ce04-4e03-aff8-0677fb3cafa3.png">
This is a example that I inputxxx, The website alreadly store my previous values xxx:
<img width="489" alt="截屏2023-04-21 上午10 07 48" src="https://user-images.githubusercontent.com/114201575/233698137-bd7ebc07-c98a-4bc7-8fbe-d2cda1547fae.png">
This is a example that I input xxx after I inputxxx:
<img width="476" alt="截屏2023-04-21 上午10 08 05" src="https://user-images.githubusercontent.com/114201575/233698162-30d8c869-d876-4ef3-9e9a-367825b604fb.png">

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
<img width="1320" alt="截屏2023-04-21 上午10 50 00" src="https://user-images.githubusercontent.com/114201575/233702277-f4ba80cb-cfab-47cb-a692-47a01c6d516f.png">

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
<img width="1315" alt="截屏2023-04-21 上午10 50 58" src="https://user-images.githubusercontent.com/114201575/233702424-8d767e23-eff8-41cb-9d7c-0485a0501bf8.png">

## part3

