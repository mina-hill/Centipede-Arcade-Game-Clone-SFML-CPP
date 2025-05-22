# Centipede Clone

A modern C++14 clone of the classic arcade game **Centipede**, built using [SFML](https://www.sfml-dev.org/) for graphics and audio. The game features a menu, instructions, scoring, and classic centipede gameplay with mushrooms, bullets, and split mechanics.

## Features

- Classic centipede gameplay: shoot the centipede as it winds through a field of mushrooms.
- Player movement and shooting (arrow keys, spacebar, or mouse click).
- Dynamic centipede splitting and direction reversal when segments are hit.
- Mushrooms (including poison and half-destroyed states) that can be destroyed for points.
- Menu system with Play, Instructions, and Quit options.
- Victory and Game Over screens with scoring.
- Background music and sound effects.

## Controls

- **Arrow Keys**: Move player
- **Spacebar** or **Mouse Click**: Shoot bullet
- **ESC**: Return to menu

## Scoring

- **Mushroom destroyed**: 1 point
- **Centipede body segment destroyed**: 10 points
- **Centipede head destroyed**: 20 points

## How to Build

1. **Dependencies**:
    - [SFML 2.5+](https://www.sfml-dev.org/download.php) (Graphics, Window, Audio)
    - C++14 compatible compiler (tested with Visual Studio 2022)

2. **Project Setup**:
    - Place all required textures in a `Textures/` folder:
        - `player.png`
        - `bullet.png`
        - `c_head_left.png`
        - `c_body_left.png`
        - `mushroom.png`
        - `halfMushroom.png`
        - `game_over.png`
        - `you_won.png`
    - Place background music in a `Music/` folder:
        - `field_of_hopes.ogg`
    - Place a font file (e.g., `arial.ttf`) in the project root.

3. **Build**:
    - Open the solution in Visual Studio 2022.
    - Ensure SFML include and lib directories are set in project properties.
    - Build and run.

## How to Play

- Select "Play Game" from the menu.
- Move your player using the arrow keys.
- Shoot at the centipede and mushrooms to score points.
- Avoid colliding with the centipede.
- The game ends in victory when all centipede segments are destroyed, or game over if the player is hit.

## Notes

- Window size and position can be adjusted in the code (`window.setSize`, `window.setPosition`).
- All assets must be present in the correct folders for the game to run.
- The game grid and logic are tuned for a 960x960 resolution but can be adjusted.

## License

This project is for educational purposes. All third-party assets (images, music, fonts) should be properly licensed for your use.

---

Enjoy playing Centipede Clone!
