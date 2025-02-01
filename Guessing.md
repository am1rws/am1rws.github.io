# Random Guessing Game Flowchart

## Description
This flowchart describes the sequence of events in a random guessing game where the computer randomly selects a number within a specified range, and the user guesses the number. The application provides feedback based on the user's input whether their guess was too high, too low, or correct.

## Diagram
```mermaid
flowchart TD
    A[Start] --> B[Generate Random Number]
    B --> C[Prompt User for Guess]
    C --> D{Is Input Valid?}
    D -->|No| E[Display Error Message]
    E --> C
    D -->|Yes| F{Is Guess Correct?}
    F -->|Yes| G[Display 'Correct' Message]
    F -->|No| H{Is Guess Too High?}
    H -->|Yes| I[Display 'Too High' Message]
    H -->|No| J[Display 'Too Low' Message]
    I --> C
    J --> C
    G --> K[End]
