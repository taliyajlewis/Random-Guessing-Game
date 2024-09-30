flowchart TD
    Start((**Start**)) --> GenerateNumber[/Generate a random number/]
    GenerateNumber --> GetUserGuess[/Get user's guess/]
    GetUserGuess --> CheckGuess[/Is the guess correct?/]
    CheckGuess -->|Yes| Correct[/Display "**Correct!** You guessed the right number."/]
    CheckGuess -->|No| IsHigher{Is the guess higher than the number?}
    IsHigher -->|Yes| High[/Display "**Too high!**"/]
    IsHigher -->|No| Low[/Display "**Too low!**"/]
    High --> GetUserGuess
    Low --> GetUserGuess
    Correct --> End((**End**))
    
    
    #This flowchart describes the actions required to complete a random number guessing game. 
    First a random number is generated anf the user is prompted to guess
    If the guess is correct the game ends and Correct, you guessed the right number is displayed.
    If the guess is in correct, a two high or two low message apprears prompting another user guest.
