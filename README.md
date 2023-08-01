
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>ShutesAndLaddersGUI
</h1>
<h3>◦ Climb Code Peaks, Slide Bug Valleys: ShutesAndLaddersGUI</h3>
<h3>◦ Developed with the software and tools listed below.</h3>

<p align="center">
<img src="https://img.shields.io/badge/C-A8B9CC.svg?style&logo=C&logoColor=black" alt="C" />
<img src="https://img.shields.io/badge/Markdown-000000.svg?style&logo=Markdown&logoColor=white" alt="Markdown" />
</p>
<img src="https://img.shields.io/github/languages/top/richardr1126/ShutesAndLaddersGUI?style&color=5D6D7E" alt="GitHub top language" />
<img src="https://img.shields.io/github/languages/code-size/richardr1126/ShutesAndLaddersGUI?style&color=5D6D7E" alt="GitHub code size in bytes" />
<img src="https://img.shields.io/github/commit-activity/m/richardr1126/ShutesAndLaddersGUI?style&color=5D6D7E" alt="GitHub commit activity" />
<img src="https://img.shields.io/github/license/richardr1126/ShutesAndLaddersGUI?style&color=5D6D7E" alt="GitHub license" />
</div>

---

## 📒 Table of Contents
- [📒 Table of Contents](#-table-of-contents)
- [📍 Overview](#-overview)
- [⚙️ Features](#-features)
- [📂 Project Structure](#project-structure)
- [🧩 Modules](#modules)
- [🚀 Getting Started](#-getting-started)
- [🗺 Roadmap](#-roadmap)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [👏 Acknowledgments](#-acknowledgments)

---


## 📍 Overview

The codebase given at https://github.com/richardr1126/ShutesAndLaddersGUI is for a graphical rendition of the board game "Chutes and Ladders", developed using the Qt framework in C++. Notably, it consists of a flexible, user-friendly GUI that allows players to create new matches with customized settings, actions such as roll, win, and undo, as well as enables users to view leaderboards. The project is exemplary in demonstrating programming principles like inheritance, strong cohesion & loose coupling, principal algorithms for turn-based games and, graphical operations of a modern GUI framework. This could serve as a considerable learning resource for software engineering students, amateur board game developers, or hobbyists taking a hands-on approach to classic board games.

---

## 🧩 Modules

<summary>Root</summary>

| File                                                                                                                 | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ---                                                                                                                  | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [marble.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/marble.cpp)                               | The provided code snippet is a C++ constructor for a class named "Marble". It's a part of the QObject parent-child system in the Qt framework. This constructor initializes Marble objects and sets their parent QObject, effectively inserting them into the QObject hierarchy.                                                                                                                                                                                                                 |
| [leaderboarddialog.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/leaderboarddialog.cpp)         | The provided code is part of a video game leaderboard display system in C++ using Qt framework. The code reads a CSV file (with player names, game wins, and total games played), stores the data into an array and calculates players' win percentages. It sorts the players by win percentage, then dynamically creates and positions labels to display the player's name, wins, total games, and win percentage for each player.                                                              |
| [leaderboarddialog.ui](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/leaderboarddialog.ui)           | The provided XML code defines a GUI Dialog titled'Leaderboard' with the dimensions 738x501 pixels, specified with a QDialog in Qt. Within the dialog box, there exists a QPushButton labeled'Close', located at position (630,460) with dimensions 100x32 pixels. The dialog does not make any connections or use any resources.                                                                                                                                                                 |
| [player.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/player.cpp)                               | This C++ code implements a Player class, mainly used in a board game setting. When an instance is created, it assigns an input username, creates an RGB color randomly, and initializes a pawn with this color. The class encapsulates functionalities like'UndoMove' and rolling dice. It has capabilities to track and change the count of'undoes' and'rerolls'. There is also an overload equality operator to compare two players.                                                           |
| [usernamesdialog.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/usernamesdialog.cpp)             | The provided code snippet represents a part of a game setup in Qt where users provide their usernames. `UsernamesDialog` constructor creates labels & text editable fields based on the `num_players_`, setting an object name for subsequent referencing. `on_startGameButton_clicked()` finds these field values and populates them in `usernames_`. If unsuccessful, it logs an error.                                                                                                        |
| [tile.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/tile.h)                                       | This coding snippet in C++ defines a Tile class in a graphic application, making it both a QObject and QGraphicsItem. The Tile has properties like coordinates (x,y), tile number, presence of shortcut, and the shortcut number. Overridden methods for boundingRect, shape, and paint aid its graphical representation. There are setter and getter functions, alongside an equals operator.                                                                                                   |
| [numplayersdiaglog.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/numplayersdiaglog.h)             | The provided code defines a'NumPlayersDialog' class inheriting from QDialog. The GUI dialog, created using Qt dialog, takes input for the number of players in a gaming scenario. It offers function'get_num_players()' to return this value. Additionally, it employs private slot'on_submitButton_clicked()' for handling a button click event.                                                                                                                                                |
| [usernamesdialog.ui](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/usernamesdialog.ui)               | The code displays a dialog box (window) with dimensions of 399x300, titled "Enter players". Within this window, there's a button named "startGameButton" situated at (290,260) point with the size of 100 by 32. The button caption text is "Start Game".                                                                                                                                                                                                                                        |
| [numplayersdiaglog.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/numplayersdiaglog.cpp)         | The provided code defines a class'NumPlayersDiaglog' containing a constructor, destructor, and a method associated with a'submitButton'. This class is a dialog window, wherein a user can select the number of players. By default, it is set to 2. On clicking the'submitButton', the value chosen by the user populates'num_players_' and the window closes.                                                                                                                                  |
| [pawn.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/pawn.h)                                       | The provided C++ code defines a `Pawn` class that's used within a graphics program (potentially a game). The `Pawn` inherits from the `QGraphicsObject`, and has functions to set/get the current tile it's sitting on, get its width, and for painting itself in a scene. It features a customizable color and a friend operator for comparison.                                                                                                                                                |
| [numplayersdiaglog.ui](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/numplayersdiaglog.ui)           | The XML code displays an'Enter players' QDialog with specific geometry and window size constraints. The dialog has a QLabel for instructing the user to input the number of players. A QSpinBox is provided for the user to select the number of players, with a minimum of 2 and maximum of 4. A QPushButton is available to submit the data.                                                                                                                                                   |
| [gamewindow.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/gamewindow.cpp)                       | The provided code represents a "Chutes and Ladders" game developed in Qt C++. Major functionalities of this game include setup controls for game initiation, game state progressing (rolling dice, moving player and switching turns), undoing previous actions, along with leaderboard management and winning scenario checks. The game also allows time tracking, player/user management, and handles elements rendering on the board.                                                         |
| [player.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/player.h)                                   | The provided code is a C++ class definition for a'Player' entity in a game involving a pawn movement on a board of tiles, likely a board game. The class methods enable aspects like setting/retrieving the player's username, undoing/rerolling a dice, checking on-board status, handling color, and rolling a dice. It also maintains records of player's previous positions and provides operations for comparisons.                                                                         |
| [pawn.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/pawn.cpp)                                   | The provided C++ code defines functionalities for a Pawn object within a graphical Qt application. The pawn has properties like current tile position (curr_tile_) and width. Triggers creation with a specified color (color_). The functions boundingRect() and shape() define the pawn’s rectangular boundary and shape (ellipse), respectively. The paint() function allows for visual rendering of the set pawn objects with specified brush used by QPainter.                              |
| [board.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/board.cpp)                                 | The code implements a method, `MakeVector()`, in the `Board` class, that organizes a 10x10 2D game'Tile' objects in a zigzag pattern, setting unique indices to each tile and storing them in a vector. Each'Tile' contains a tile number corresponding to its order in the vector.                                                                                                                                                                                                              |
| [chutesAndLadders.pro.user](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/chutesAndLadders.pro.user) | This XML code is a project configuration file for a project built with QtCreator IDE. It specifies important details about environment variables, project settings, editor settings, plugin settings, and targeted platforms. These details model software behavior like indentation styles, file encodings, active test frameworks, the build directory path and further specifications for build configurations of Debug, Release, and Profile modes.                                          |
| [gamewindow.ui](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/gamewindow.ui)                         | This XML code represents the GUI layout of a game called "Chutes and Ladders". The GUI includes a main window with a set size and widgets such as buttons for starting, ending, rolling, undoing actions, and quitting the game, labels for displaying dice results and current player information, and board.                                                                                                                                                                                   |
| [tile.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/tile.cpp)                                   | The code describes functionalities of a "Tile" in a certain application (e.g., game), likely a 2D graphics display. When initialized, every tile gets X, Y coordinates, width, and predefined stand-in integers for potential use. The boundingRect() provides a square area indicating tile's spatial aspect. The shape() method describes a rectangular shape using the path fill. The paint() function colors the tile. An overloaded operator checks if two tiles have the same coordinates. |
| [marble.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/marble.h)                                   | The provided code snippet is the header file for a simple class, named'Marble', in C++. This class is derived from the QObject base class, inherent in the Qt framework. Currently, the content only includes a default constructor, accepting a QObject pointer as optional parent input, and an empty signals section indicating that Marble is capable of sending signals, allowing for event-driven programming.                                                                             |
| [leaderboarddialog.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/leaderboarddialog.h)             | This code defines a LeaderboardDialog class, a Qt dialog window, with main functionalities: (1) Reading files with the `ReadFile` method, an operation likely related to leaderboard data handling. (2) Interaction event handling with a GUI component or QPushButton responsible for executing a function when clicked, handled by the `on_pushButton_clicked` slot. The `total_players` attribute may track the total number of players retrieved or displayed.                               |
| [board.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/board.h)                                     | The code define a Board class-based on QGraphicsScene, for a 10x10 tile-based board game in a Qt based GUI application. The Board provides functions like at() to access individual tiles from a 2D array, SetTileAt() to set a tile to a specified position on the board, and MakeVector(). It maintains a separate vector list of all the tiles.                                                                                                                                               |
| [usernamesdialog.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/usernamesdialog.h)                 | The provided code defines a class `UsernamesDialog` derived from `QDialog` within a Qt interface. The class constructor accepts a parent widget and the number of players. It consists of a function `get_usernames()` to fetch users. It also contains a pointer to its user interface, the number of players, and a vector to store usernames. Private slot `on_startGameButton_clicked` is connected to the game start button.                                                                |
| [main.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/main.cpp)                                   | This code snippet is the main function of a Qt-based application which includes a'GameWindow' component. First, it seeds the random number generator using the current time in milliseconds, which helps ensure randomness in gameplay. It then launches a Qt application instance, initializes a'GameWindow', and displays it by calling'show()'. The program then enters the primary event loop by calling'a.exec()'.                                                                          |
| [gamewindow.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/gamewindow.h)                           | The provided code defines the "GameWindow" class for a GUI-based game. It helps to manage the game functionalities like maintaining player objects, switching current player, initiating and resetting the game, and checking game win conditions. It also provides reactions to various button actions (start/end/undo game, roll, move) and functions relating to a game countdown timer.                                                                                                      |


---

## 🚀 Getting Started

### ✔️ Prerequisites

> This program is meant to be built with Qt Creator.


## 🤝 Contributing

Contributions are always welcome! Please follow these steps:
1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.
2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.
3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).
```sh
git checkout -b new-feature-branch
```
4. Make changes to the project's codebase.
5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.
```sh
git commit -m 'Implemented new feature.'
```
6. Push your changes to your forked repository on GitHub using the following command
```sh
git push origin new-feature-branch
```
7. Create a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.
The project maintainers will review your changes and provide feedback or merge them into the main branch.

