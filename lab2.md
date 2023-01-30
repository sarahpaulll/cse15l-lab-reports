# Lab Report 2

## Part One
The code for StringServer is shown below along with two images of adding strings to the server.

![StringServer](https://user-images.githubusercontent.com/122580017/215230190-6cdd453b-be36-4a0a-a02f-ea8745f16997.png)

The image below demonstrates good morning being added to the StringServer. By adding /add-message?s=Good Morning after the server port, this calls the main method in the class StringServer, which then calls the handleRequest method. The handleRequest method uses localhost:5898/add-messages?s=Good Morning as its argument. By calling handleRequest with the path add-messages?s=Good Morning it changes the instance variable string from " " to "Good Morning" as a result of the if statement on the 19th line. Then after setting the instance variable string to Good Morning it returns the string Good Morning.  
![String1](https://user-images.githubusercontent.com/122580017/215230244-949791b4-769d-48dc-ade5-650aebca4cbd.png)

The image below demonstrates when another string is added to the StringServer. The first method which is called is the main in the class StringServer. Main then calls the method handleRequest which uses localhost:5898/add-messages?s=Hello as its argument. By calling handleRequest with this argument it changes the instance variable string from "Good Morning" to "Good Morning\nHello" which is shown in the 24th line. After the instance variable string is updated it then returns this string, therefore resulting in the image below. 
![String2](https://user-images.githubusercontent.com/122580017/215230254-4be85352-4f39-49d3-ac48-528831a22adb.png)

## Part Two

**Bugs**
```
# method reversed with bug
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
}
```
```
# JUnit test with failure-inducing input 
@Test
public void testReversed() {
    int[] input2 = {1, 2, 3, 4, 5};
    assertArrayEquals(new int[] {5, 4, 3, 2, 1}, ArrayExamples.reversed(input2));
}
```
```
# JUnit test without failure-inducing input 
@Test
public void testReversed() {
    int[] input1 = {0};
    assertArrayEquals(new int[]{0}, ArrayExamples.reversed(input1));
}
```
**Running the Tests**

![Running Tests](https://user-images.githubusercontent.com/122580017/215299291-23384dc3-7576-48f1-94b4-29c63c25676f.png)
![Running Tests](https://user-images.githubusercontent.com/122580017/215299667-ef4ea61d-57ff-4e2a-9466-5b89ec574cd4.png)

**The Bug Before-and-After Code**
```
# before
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
}
```
```
# after
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
}
```
The bug was that the code was copying the reversed version of the newArray, which is initialized to all zero entries, into the original array. The changes to fix the bug were made in the fourth line of the code where newArray[i] is now on the right side of the equal sign and arr[arr.length - i -1] on the left side and then returning newArray. Thus, now the code copies the original array in reversed order into the newArray and then returns this newArray. 

## Part Three
In lab two I learned how to use Github Desktop, which I was unfamiliar with before this lab. On Github Desktop I learned how to clone respitories from my github account and open these files onto VSCode where I could edit them. After editing these files, I learned how to commit and push these changes on Github Desktop so that the changes within the file would be visible on Github. 
