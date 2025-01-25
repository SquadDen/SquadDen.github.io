# Number Guessing game FlowChart
```mermaid 
flowchart TD
A[Start] --> B{Generate Random Number}
B--> C[Input Guess from User]
C--> D{Valid Number?}
D-->|No| E['Invalid number' Message]
E--> C
D -->|Yes| F{Correct?}
G --> C
F-->|Yes| G[Display 'Correct Guess' Message]
F -->|No| H{'Too high?'}
H-->|yes| I[display 'Too High' Message]
H-->|No| J[Display 'Too Low' Message]
I--> C
J --> C
G --> K[End]


