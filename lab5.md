Hello, I am using the Windows operating system. I have 1 failure after running the jUnit test on the reverseInPlace method in the ArrayExamples.java. There might be something wrong with my implementation of the reverseInPlace method. 
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
