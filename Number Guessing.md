# Number Guessing game FlowChart
This is a flowchart I've created for the concept of my Number **Guessing** game. 
## The Instructions of the game
+ Generate a random number between 1-5
+ Guess a number beween 1 and 5
+ If the number isn't within the requirements an error message will display
+ if the number is within the requests then it will check if its correct
+ if it's incorrect it will display either too high or too low. If it's correct it will say correct guess.
```mermaid 
flowchart TD
A[Start] --> B{Generate Random Number}
B--> C[Input Guess from User]
C--> D{Is Input Between 1 and 5?}
D-->|No| E[Display 'Invalid number' Message]
E--> C
D -->|Yes| F{Correct?}
F-->|Yes| G[Display 'Correct Guess' Message]
F -->|No| H{'Too high?'}
H-->|yes| I[display 'Too High' Message]
H-->|No| J[Display 'Too Low' Message]
I--> C
J --> C
G --> K[End]


