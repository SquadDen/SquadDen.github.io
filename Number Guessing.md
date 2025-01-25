# Number Guessing game FlowChart
```mermaid 
flowchart TD
A[Start] --> B{Generate Random Number}
B--> C[Input Guess from User]
C--> D{Valid Number?}
C--> E{Invalid Number}
D-->|No| E[Invalid Input Message]
D -->|Yes| F{Correct?}
E --> G[Display 'Invalid Input' Message]
G --> C
F-->|Yes| G[Display 'Correct Guess' Message]
F -->|No| H{'Too high?'}
H-->|yes| I[display 'Too High' Message]
H-->|No| J[Display 'Too Low' Message]
I--> C
J --> C
G --> K[End]


