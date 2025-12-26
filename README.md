# Java Casino Application 🎰

A full-featured casino GUI application built entirely with standard Java libraries. Play Blackjack, Baccarat, and War with secure password hashing and persistent account management.

## Features

- **Three Casino Games**: Blackjack (with split/double down), Baccarat (Punto Banco), and War
- **Secure Authentication**: SHA-256 password hashing with random salt generation
- **Account Management**: User registration, login, and real-time balance tracking
- **Pure Java**: No external dependencies - uses only `javax.swing`, `java.awt`, `java.io`, `java.security`, and `java.util`
- **Persistent Storage**: Automatic save/load of encrypted user data

## Requirements

- Java JDK 8 or higher
- No external libraries required

## Quick Start
```bash
# Clone the repository
git clone https://github.com/yourusername/java-casino.git
cd java-casino

# Compile
javac *.java

# Run
java Main_Menu
```

## How to Play

1. **Register** a new account with username, password, and starting balance
2. **Login** with your credentials
3. **Select a game** (Blackjack, Baccarat, or War)
4. **Place your bet** and follow on-screen instructions
5. Balances are **automatically saved** after each round

## Game Rules Summary

- **Blackjack**: Get closer to 21 than dealer. Blackjack pays 3:2. Split, double down, and insurance available.
- **Baccarat**: Bet on Player (1:1), Banker (0.95:1), or Tie (8:1). Uses 8-deck shoe with authentic drawing rules.
- **War**: Higher card wins. Ties trigger "War" - double your bet or surrender for 50% back.

## Security

- SHA-256 password hashing with unique 16-character salts per user
- No plaintext passwords stored
- User data saved in `Player_info.txt` as: `username,hashedPassword,salt,balance`

## Files

- `Main_Menu.java` - Entry point and login system
- `Player.java` - Account management and authentication
- `Cards.java`, `Deck.java`, `CardPanel.java` - Card system
- `BlackjackGameWindow.java`, `BaccaratGameWindow.java`, `WarGameWindow.java` - Game implementations
- `ViewCardsWindow.java` - Deck visualization



---

*Educational purposes only. No real money involved.*
