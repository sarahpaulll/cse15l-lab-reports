# Lab Report 4

## Step One: Log into ieng6
 
![SSH](https://user-images.githubusercontent.com/122580017/221382912-67ccba61-10ba-4ce2-9559-218b8e15ebb0.png)

Keys Pressed: `ctrl -R ssh <enter>`

The `ssh cs15lwi23awe@ieng6.ucsd.edu` command was already in the search history so I used `ctrl -R` command, which searches the command history, to access it. 

## Step Two: Clone your fork of the repository from your Github account

![clone](https://user-images.githubusercontent.com/122580017/221383116-4ff9d90f-b80c-44b6-8a47-e8d9b3897b75.png)

Keys Pressed: `git clone ctrl -V <enter>`

To clone the fork of the repository I copied the ssh link from my lab7 repository then the `ctrl -V` command pastes the copied link into the terminal. 


## Step Three: Run the tests, demonstrating that they fail

![run](https://user-images.githubusercontent.com/122580017/221383266-879e276c-3270-43ac-856b-8f9dde5f5e95.png)

Keys Pressed: `cd lab7`, `ctrl -R javac <enter>`, `ctrl -R java <enter>`

To run the tests I typed `cd lab7` in order to be in the correct directory (lab7). Then since the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` and `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` commands were already in the search history I used ctrl -R to search my command history to find the desired commands.

## Step Four: Edit the code file to fix the failing test
![nano](https://user-images.githubusercontent.com/122580017/221383368-ff5b5982-65a1-4b2a-a8bd-4c971a4b78fb.png)

![ctrl -w](https://user-images.githubusercontent.com/122580017/221383391-f2ae3777-01b2-4b60-870b-359afe59f118.png)

![fix](https://user-images.githubusercontent.com/122580017/221383496-c5d1a5c0-0d1d-4fb6-8b88-0634178443b4.png)

Keys Pressed: `nano L<tab>.j<tab> <enter>`, `ctrl -W merge <enter>`, `<down>` 19 times, `<left>` 6 times, `<delete> 2`, `ctrl -O <enter>`, `ctrl -X`

By using `<tab>` this autocompletes the word to ListExamples.java. The command `ctrl -W` searches through the file to find the given word, which in this case was merge. The `<down>` and `<left>` commands brought the cursor to the desired line that had the error in it. To fix the error I clicked `<delete> 2` which changed `index1` to `index2` in the last while loop of the merge method. `ctrl -O` saves the changes and `ctrl -X` exits the file. 


## Step Five: Run the tests, demonstrating that they now succeed
 
![run](https://user-images.githubusercontent.com/122580017/221384401-1f59cfe4-d7e8-4cc5-a9ab-8df0c8ebbb56.png)

Keys Pressed: `<up><up><up><enter>`, `<up><up><up><enter>`

The `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command was three up in the search history so I used the up arrow to access it. Then the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` was also three up in the search history so I used the up arrow to access it. 


## Step Six: Commit and push the resulting change to your Github account 

![commit and push](https://user-images.githubusercontent.com/122580017/221384685-e8ab7990-4881-43ae-b681-eb4abda4077a.png)

![github](https://user-images.githubusercontent.com/122580017/221385053-100d03b9-d9ec-4c72-a9ef-a0b9165a9352.png)

Keys Pressed: `git add L<tab>.j<tab> <enter>`, `git commit -m "updated" <enter>`, `git push ctrl -V <enter>`

By using `<tab>` this autocompletes the line to ListExamples.java. To push the changes to github I copied the lab7 repository ssh link then `ctrl -V` pastes the copied link into the command line. 
