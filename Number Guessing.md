# Number Guessing game FlowChart
```mermaid 
flowchart TD
A[Start] --> B{Generate Random Number}
B--> C[Input Guess from User]
C--> D {Valid Number?]
D--> | No| E[Invalid Input Message]

[End]

