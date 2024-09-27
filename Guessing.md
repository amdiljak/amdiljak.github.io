Explanation of the Flowchart  
Start: The game begins.  
Player makes a guess: The player inputs their guess.  
Is the guess correct?: The game checks if the guess is right.  
If Yes, the player wins.  
If No, the game checks if the guess is too high or too low.  
Too high / Too low: The game provides feedback and loops back to the guess step.  
Play again?: After winning, the player can choose to play again or end the game.  

```mermaid
flowchart TD
    A[Start] --> B[Generate random number]
    B --> C[Player makes a guess]
    C --> D{Is the guess correct?}
    D -- Yes --> E[Player wins!]
    D -- No --> F{Is the guess too high or too low?}
    F -- Too high --> G[Tell player: Too high!]
    F -- Too low --> H[Tell player: Too low!]
    G --> C
    H --> C
    E --> I[Play again?]
    I -- Yes --> A
    I -- No --> J[End]    
