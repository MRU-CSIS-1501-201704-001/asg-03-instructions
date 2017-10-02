# Assignment 03: Getting Iffy with It

## Superfun Quiz Challenge

_Pop quiz, hotshot._

---

_I think that random trivia is fun. If you combine that with the utter joy of multiple-choice questions, you get the Superfun Quiz™:_

Entomology is the science that studies  
A.	Behavior of human beings  
B.	Insects  
C.	The origin and history of technical and scientific terms  
D.	The formation of rocks  

Eritrea, which became the 182nd member of the UN in 1993, is in the continent of  
A.	Asia  
B.	Africa  
C.	Europe  
D.	Australia  

Which of the following is not one of the bots on Mystery Science Theater 3000?  
A.	Jambot  
B.	Gypsy  
C.	Tom Servo  
D.	Crow T. Robot  

Germany signed the Armistice Treaty on ____ and World War I ended  
A.	January 19, 1918  
B.	May 30, 1918  
C.	November 11, 1918  
D.	February 15, 1918  

The headquarters of the United Nations are situated at  
A.	New York, USA  
B.	Hague (Netherlands)  
C.	Geneva  
D.	Paris  

What utensil serves as the rallying cry of The Tick?  
A.	chopstick  
B.	spoon  
C.	fork  
D.	butter knife  

What is the theme of the board game Die Macher?  
A.	sculpting  
B.	car racing  
C.	German politics  
D.	castle building  

_Whew, I hope you can handle the fun!_

---

**MAKE THIS HAPPEN:**

Write code that does the following:

1. For each of the questions above:
    * Display the question.
    * Display the answers.
    * Ask the user for an answer.
1. As the questions are answered, the program must keep track of the number of correct answers.
1. Also keep track of the number of C answers that the user entered.
1. After all of the questions have been answered, output something like one of the following sentences:
    * `You have passed the quiz!`
    * `You have failed the quiz.`
    * The automated tests will look for “pass” or “fail” in your output.
1. If the user entered all C answers, the program should also print:
    * `All Cs, eh? That’s how I passed music theory last year.`
    * The automated tests will look for “Cs” in your output.

**NOTES:**

* You'll have to determine the correct answers to the quiz.
* The user passes the quiz if they have at least 5 correct answers.
* The user must be able to enter their answers as an uppercase or lowercase letter.
* The answers must be stored in char variables and compared to another char in the if statements.
* To check answers correctly, you can either use conditional operators or get some help from either Java's `String` or `Character` classes. Your choice. (I won't dock marks for using either method, but practicing going to the API is important.)
