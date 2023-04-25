Part 1:
Step 1: create the code like this:
![Capture](https://user-images.githubusercontent.com/130394449/234158985-8afc222d-0fa2-45e6-b744-7c82b418bbd3.PNG)

Step 2: open the terminal in visual studio code and enter the command "javac Server.java StringServer.java" and "java StringServer 4000" and you will get the url to the website you created like this:

![Capture1](https://user-images.githubusercontent.com/130394449/234159174-564b6475-acbe-429c-9c21-5b9feab3fc8d.PNG)

Step 3: enter the URL in a browser like this:

![Capture2](https://user-images.githubusercontent.com/130394449/234159408-ca34c354-d7bc-476c-b970-1fa19aa8a7c5.PNG)

This main method and handlerRequest method are called and the url you enter in the browser is taken as the argument. The str field equals to the output shown in the website, which is nothing right now. The Port field equals to 4000.
You will see nothing at first. Then you can change your url by adding "/add-message?s=<string>" to the end of the url. We will try to add "/add-message?s=Hello" first and you will see "Hello" pop up in the website like this:
  
![Capture3](https://user-images.githubusercontent.com/130394449/234159796-a57502b1-8699-4c9e-bcb3-6080bc846a0f.PNG)

This main method and handlerRequest method are called and the url you enter in the browser is taken as the argument. The str field equals to the output shown in the website, which changes to "Hello" right now. The Port field equals to 4000.
Then we will change the url by adding "/add-message?s=How are you". You will see "Hello" and "How are you" poping up on the line below "Hello" like this:
  
![Capture4](https://user-images.githubusercontent.com/130394449/234160386-ffb5840d-38fb-4358-8a5f-9f9e4e70cd34.PNG)

This main method and handlerRequest method are called and the url you enter in the browser is taken as the argument. The str field equals to the output shown in the website, which changes to "Hello\nHow are you" right now. The Port field equals to 4000.

Part 2:
A failure-inducing input:
```
  @Test
  public void testReversed1() {
    int[] input1 = { 5,8,7,6};
    assertArrayEquals(ArrayExamples.reversed(input1), new int[]{6,7,8,5});
  }
  ```

An input that doesn’t induce a failure:
```
  @Test
  public void testReversed2() {
    int[] input1 = {0,0,0,0};
    assertArrayEquals(ArrayExamples.reversed(input1), new int[]{0,0,0,0});
  }
  ```

The symptom:

<img width="1017" alt="Screen Shot 2023-04-24 at 10 45 45 PM" src="https://user-images.githubusercontent.com/130394449/234185238-9ee6f9b9-b30f-4d78-8fe4-70922e76f305.png">


The bug:
before changes:
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
  ```
 
 after changes:
 ```                           
 static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    int j=0;
    for(int i = arr.length-1; i >=0; i -= 1) {
      newArray[j] = arr[i];
      j++;
    }
    return newArray;
  }
  ```
My code works because it sets the last elements of the original array as the first element of the new array. The second last element of the original array as the second elements of the new array. So on and so forth.

part 3:
I learned about debugging. I learned how to find bugs and fix bugs.
I learned about how to make my own URL with java code.
I learned different parts of an URL and their meanings.
