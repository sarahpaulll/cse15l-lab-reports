# Lab Report 4

## Step One: Log into ieng6
The `ssh cs15lwi23awe@ieng6.ucsd.edu` command was already in the search history so I used `ctrl -r ssh <enter>` to access it.  

![SSH](https://user-images.githubusercontent.com/122580017/221382912-67ccba61-10ba-4ce2-9559-218b8e15ebb0.png)


## Step Two: Clone your fork of the repository from your Github account
To clone the fork of the repository I copied the ssh link from my lab7 repository then typed `git clone ctrl -v <enter>`

![clone](https://user-images.githubusercontent.com/122580017/221383116-4ff9d90f-b80c-44b6-8a47-e8d9b3897b75.png)


## Step Three: Run the tests, demonstrating that they fail
To run the tests I typed `cd lab7` in order to be in the correct directory. Then because the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` and `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` commands were already in the search history I used ctrl -r to search the bash history. To run these commands in the screenshot I typed `ctrl -r javac <enter>` then `ctrl -r java <enter>`

![run](https://user-images.githubusercontent.com/122580017/221383266-879e276c-3270-43ac-856b-8f9dde5f5e95.png)


## Step Four: Edit the code file to fix the failing test
First to edit the code file I used the command `nano L<tab>.j<tab> <enter>`. Once in the nano file I used the command `ctrl -w merge <enter>` in order to locate the merge method. Then to get to the error I hit `<down>` 19 times then `<left>` 6 times. To fix the error I hit `<delete> 2` which changed `index1` to `index2` in the last while loop of the merge method. Then to save the changes I hit `ctrl -o <enter>` and to exit I did `ctrl -x`.

![nano](https://user-images.githubusercontent.com/122580017/221383368-ff5b5982-65a1-4b2a-a8bd-4c971a4b78fb.png)

![ctrl -w](https://user-images.githubusercontent.com/122580017/221383391-f2ae3777-01b2-4b60-870b-359afe59f118.png)

![fix](https://user-images.githubusercontent.com/122580017/221383496-c5d1a5c0-0d1d-4fb6-8b88-0634178443b4.png)


## Step Five: Run the tests, demonstrating that they now succeed
To run the tests I used the commands `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` and `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` which were already in my search history so to run them in the image below I typed `<up><up><up><enter>` and `<up><up><up><enter>` into the terminal.
 
![run](https://user-images.githubusercontent.com/122580017/221384401-1f59cfe4-d7e8-4cc5-a9ab-8df0c8ebbb56.png)


## Step Six: Commit and push the resulting change to your Github account 
I first entered `git add Listexamples.java` into the terminal by typing `git add L<tab>.j<tab> <enter>`. Then I typed `git commit -m "updated" <enter>` into the terminal. Lastly to push the changes to github I copied the lab7 repository ssh link and typed `git push ctrl -v <enter>` into the terminal.

![commit and push](https://user-images.githubusercontent.com/122580017/221384685-e8ab7990-4881-43ae-b681-eb4abda4077a.png)
![github](https://user-images.githubusercontent.com/122580017/221385053-100d03b9-d9ec-4c72-a9ef-a0b9165a9352.png)

