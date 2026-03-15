## Emoji Sudoku

A SwiftUI-based iOS application that reimagines the classic Sudoku puzzle by replacing standard numbers with emojis. The application features a custom user interface designed to mimic a retro handheld console using flat design principles.

## Features

- **Flat Design Interface**: Implements a "machine within a machine" visual style. The UI relies on solid colors, thick borders, and lacks gradients or shadows, aligning with neo-brutalism and retro console aesthetics.
- **Dynamic Puzzle Generation**: Utilizes a Depth-First Search (DFS) algorithm to programmatically generate unique and solvable Sudoku grids upon initialization, ensuring a different puzzle layout for every session.
- **Game Modes**:
  1. **一般模式**: Uses 9 distinct, everyday emojis.
  2. **主題模式**: Uses 9 emojis from a unified category (e.g., animals, fruits, or vehicles).
  3. **混亂模式**: Uses 9 emojis with similar colors or geometric shapes to increase visual difficulty.
- **Life System**: Players are allocated 5 lives per session. Incorrect placements decrement the life counter, leading to a game over condition if depleted.
- **Time Tracking**: Features a built-in timer. The fastest completion time for each game mode is persistently stored locally using `UserDefaults`.
- **Audio Integration**: Manages background music and UI interaction sound effects via `AVFoundation`.
- **Smart Input Assist**: The lower input matrix tracks the frequency of placed emojis. Once an emoji is correctly placed 9 times on the board, its corresponding input button becomes hidden, and the system automatically selects the next available emoji.

## Tech Stack

* **Framework**: SwiftUI
* **Architecture**: MVVM (Model-View-ViewModel)
* **Concurrency / Reactive Programming**: Combine (Timer publishing)
* **Media Framework**: AVFoundation (Audio playback)
* **Local Storage**: UserDefaults

## Requirements

- iOS 16.0+
- Xcode 14.0+
- Swift 5.0+

## Installation & Setup

1. Clone the repository to your local machine:
   ```bash
   git clone [https://github.com/YourGitHubUsername/YourRepositoryName.git](https://github.com/YourGitHubUsername/YourRepositoryName.git)
