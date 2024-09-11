# PROJECT 2 - Chatbot

### Name

_Write your name here_

### Introspection

_Describe the challenges you faced and what you learned_

### Resources

_List the people and resources you used to complete the project_

This will be your first programming project! Read this README carefully and follow the instructions.


### *DO NOT EDIT BELOW THIS LINE*
---


## Goal

The goals of this project are:

* To start using `.py` files for running code
* Use `expressions`, `variables`, `conditionals`, `input`, and `string` manipulation to interact with users.

## Description

In this first project, you will create a chatbot! This chatbot will interact with users and perform a variety of tasks based on user input. You will also add personalization so that each interaction is different and provides a persona to the chatbot.

Following are the main tasks for this project, I would suggest completing them in sequence.

### `.py` File

The chatbot code should be in a `.py` file. So far we have been using `.ipynb` or Jupyter notebooks but now we want to start using `.py` files. There are two ways to create a `.py` file in VS Code.  

Option 1:

1. Click on File > New File > Select "Python File" from the drop-down box.
2. Click on File > Save > Name it "chatbot". The `.py` extension should be pre-written in the name.

Option 2:

1. Press Cmd/Ctrl + N. This will open a new tab
2. Press Cmd/Ctrl + S, name the file `chatbot.py`


### Personalization

The chatbot should ask for user's name and other information, such as your place of origin, favorite movie, or your deam vacation city, to make the interactions personal. Think about what would **you** like a chatbot to know about yourself to make the interactions personal. These questions should be asked at the beginning of the interaction and until the chat is ended, the chatbot should remember these details. As you complete the tasks below, think how you can use the information you asked to personalize the interaction. You can use them in one of the math or string operations.

```bash
# Simple questions to ask to seem personal
> Hello, I am chatbot, what is your name?
VJ
> Hello VJ, lovely to meet you! Where are you from?
Texas
> Oh wow! I have always wanted to go to Texas!
```

### Persona

The chatbot should also have its own persona to make interactions human. Think about your favorite movie/TV/game/book character. You can model the responses of the chatbot as if that character is responding. Here are a few ways to provide persona - you can name your chatbot, choose the style/slang of the chatbot in which it responds. You can improve personalization by imagining an interaction between you and your favorite character.

```bash
# I imagining my chatbot to be Sheldon Cooper from The Big Bang Theory
> Sheldon: Hi! I am Dr. Sheldon Cooper, B.S., M.S., M.A., Ph.D., ScD.... OMG Haha! What about you, what is the highest level of education you have? BS, MS, or PhD?
BS
> Sheldon: Hmm! So I am talking to a 10-year-old child. Alright, kid what is your name?
VJ
> Sheldon: Hello kid VJ. 
```

```bash
# I can also differentiate the initial response of my chatbot based on the first input
> Sheldon: Hi! I am Dr. Sheldon Cooper, B.S., M.S., M.A., Ph.D., ScD.... OMG Haha! What about you, what is the highest degree of education you have? BS, MS, or PhD?
PhD
> Sheldon: Ohh! A fellow science lover. What is your name friend?
VJ
> Sheldon: Hello friend VJ!
```


### Menu

After asking the first few personalization questions, print a menu option listing the things your chatbot can do. These things can be mathematical operations, string operations, math, or word games. You should then ask the user to choose an option from the menu and then perform that thing.

```bash
# Simple version
...
> What can I help you today with? 
1: Add two numbers
2: Multiply two numbers
3: Subtract two numbers
4: Count the letters in a word
5: Check the number of a specific letter in a word
6: Reverse the word
```


```bash
# Sheldon version_1
...
> Sheldon: Hello kid VJ. 
> Sheldon: Choose one of the following option, kiddo:
A: Compute the sum of two numbers
B: Reverse a string
C: Multiply two numbers
D: Inspire you
```

```bash
# Sheldon version_2
...
> Sheldon: Hello friend VJ!
> Sheldon: Choose one of the following option, friend:
A: Compute the sum of two numbers
B: Reverse a string
C: Multiply two numbers
D: Inspire you
```

### Mathematical operations

There should be _at least_ 3 mathematical operations that the chatbot should do. These operations can be simple things like finding out if a number is odd or not, computing factorial, rounding operations, or checking if it is prime or not.

```bash
# Simple version
...
1
> Sure, VJ. I can add two numbers. Give me the first number
10
> Ok, now give me the second number
15
> The result of 10 and 15 is 25
```

```bash
# Sheldon version_1
...
C
> Sheldon: Sure kiddo VJ, give me the first number
2
> Sheldon: Now give me the second number
3
> Sheldon: The product of 2 and 3 is 6, kiddo VJ.
```

```bash
# Sheldon version_2
...
C
> Sheldon: Sure friend VJ, give me the first number
2
> Sheldon: Now give me the second number
3
> Sheldon: The product of 2 and 3 is 6, friend VJ.
```


### String operations

There should be _at least_ 3 string operations that the chatbot should do. These operations can be converting string into upper/lower case letters, counting instances of a specific letter, reversing them, jumbling them, or even if they are palindromes or not.


```bash
# Simple version
...
4
> Of course, VJ. I can count letters. What is the word
strawberry
> strawberry has 10 letters
```

```bash
# Sheldon version_1
...
D
> Sheldon: Ok kiddo VJ, tell me your favorite quote and I will inspire you
never give up
> Sheldon: NEVER GIVE UP KIDDO VJ!!!!!
```

```bash
# Sheldon version_2
...
D
> Sheldon: Ok friend VJ, tell me your favorite quote and I will inspire you
just do it
> Sheldon: JUST DO IT FRIEND VJ!!!!!
```

### Input validation

For every math or string operation that the user selects, verify that the input provided by the user for that specific operation is valid. When asking for numbers for a mathematical operation, check if the user actually provides number or not. If the user does not provide a number, ask again. Similarly for string operations, if the user provides an invalid string then ask the user to provide you with a valid string.

```bash
# Simple version
...
1
> Sure, VJ. I can add two numbers. Give me the first number
10
> Ok, now give me the second number
Blue
> Oops, Blue is not a number, give me a number
5
> The result of 10 and 15 is 25
```

```bash
# Sheldon version_1
...
C
> Sheldon: Sure kiddo VJ, give me the first number
2
> Sheldon: Now give me the second number
H
> Sheldon: Kiddo VJ, you have a BS, you should know H is not a number. Try again
5
> Sheldon: The product of 2 and 5 is 10, kiddo VJ.
```

```bash
# Sheldon version_2
...
D
> Sheldon: Ok friend VJ, tell me your favorite quote and I will inspire you
5512
> Sheldon: Friend VJ, you have a PhD, you should know that 5512 is not a quote. Give me a quote and I will inspire you.
dare northward
> Sheldon: DARE NORTHWARD FRIEND VJ!!!!!
```


## Extra Credit

Following tasks are for extra-credit

### Better Input Validation

I would expect students with more programming experience to implement better input validation throughout the interaction with the chatbot. They should be able to handle all types of inputs at any stage of interaction and ensuring it does not result in an error.

### Math games

Write simple and fun math games. These games can be guessing a number, quizzing the user on their arithmetic, and so on. Use your creativity to write fun games. You can also think that you are creating math games for kids who are just starting to learn how to do basic arithmetic. For example, asking the user (assuming they are a kid) to add two single-digit numbers. If they get the response correctly, congratulate them, if not, provide the answer and encouragement. You can also try to increase the complexity of the games depending on who would be using this.

### Word games

Similar to math, think about what fun word games can you write for kids, for example, you can ask them to guess the missing letters of a word, how many specific letters in a given word, and so on. You can also write more complex games for adults, such as a version of the Wordle game by asking the user to guess the word chatbot is thinking and then provide them N guesses, after each guess give them hints on the letters that were correct. You can create a lot of variations of these games. 

### Formatted printing

I expect that the students with prior programming experience should provide better formatting of the input and output in the terminal. Use f-strings to format the number of decimal points printed is clean, there are proper spaces and new lines between each interaction. You can also look into adding color to the text.

### Continous Interaction

After you complete one interaction with the chatbot, the chatbot should print the menu again until the user chooses an option to end interaction.

## Rubric

* Personalization - 10 points
* Persona - 10 points
* Menu - 5 points
* Math Operations - 30 points
* String Operations - 30 points
* Input Validation - 15 points

* Extra Credit - 2 points for each task

In each aspect of the task, points will be given for creativity and imagination

## Tips On How To Excel


### General Advise

* Start early!
* Ask for help when stuck. Remember the 30 minute rule? No? Look into the syllabus.
* Break down the task into smaller tasks and try to implement them in Jupyter Notebook. Once implemented in the notebook successfully, transfer it into `.py` file.
* Run the `.py` file to make sure the new addition did not break any changes.
* After implementing each small task, commit changes.
* Review the notebooks from classes available on GitHub if you cannot remember syntax for anything.
* Run your code multiple times and vary the inputs to ensure it works as intended. 

### Project-Specific Advise

* First try to finish a simpler version of the chatbot with simple math expressions and simple string manipulation.
* Next, enhance personalization by asking unique questions and saving the answers and think about where to include them in your responses.
* Ask your peers to interact with your chatbot. You can borrow **ideas** (**not code**) but try to make them your own.

## Feedback

