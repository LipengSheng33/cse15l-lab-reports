Part I:

Student question:
I am using the Windows operating system. I have 1 failure after running the jUnit test on the reverseInPlace method in the ArrayExamples.java. There might be something wrong with my implementation of the reverseInPlace method. 
This is the code:

```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
  ```
  
  I wrote a test like this:
  
  ```
   @Test
  public void testReversed1() {
    int[] input1 = { 5,8,7,6};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{6,7,8,5}, input1);
  }
  ```
  
  And I got failures like this:
  
  ![Capture1](https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/b50827bc-5ac2-4320-b517-adb1d570e273)

The input that the reverseInPlace took as an argument is an array of integers {5, 8, 7, 6}. After calling the reverseInPlace method, it should return 6, 7, 8, 5.
Therefore, I expect 8 at index 2, but instead the result is 7.

TA answer:
What happens when i is larger than half of the length of the array?
Try saving the first element as an int type and then save the value of the last element of the array to the first element and then save the value of the int type to the last element. The for loop should only loop through half the length of the array because we are changing the values from the start and the end at the same time and we do not want to change the value again.

My code after taking the advice of the TA: 

```
static void reverseInPlace2(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int temp = arr[i];
      arr[i] = arr[arr.length-i-1];
      arr[arr.length-i-1]=temp;
    }
  }
  ```

My result after calling my bash scripts that runs the jUnit test:

![Capture2](https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/a0517f32-4709-4243-81ef-a935e249d8fa)

This is a screenshot of my bash script:

![Capture3](https://github.com/LipengSheng33/cse15l-lab-reports/assets/130394449/edbf1f9c-593a-427e-8f40-4b244e9030a7)

The bug of the original code is that it did not save the values of the original array so that after the midpoint, it cannot get the values of the first half of the array. We can see from the terminal output above when the Junit test produced a failure that it was the element at index 2 that went wrong, which is the first element after the midpoint. Therefore, I found out that the code went wrong after the for loop reach the midpoint.

Part II:

The most exciting thing I learned during the second half of this quarter that I did not know before is the bash script. With the bash script, I can run so many command at the same time without typing them into the terminal one by one, which is much more convienient. Also, bash is a very concise and interesting programming language and I really like writing it.
