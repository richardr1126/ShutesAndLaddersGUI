
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>ShutesAndLaddersGUI
</h1>
<h3>◦ Scaling up the fun, one ladder at a time!</h3>
<h3>◦ Developed with the software and tools listed below.</h3>

<p align="center">
<img src="https://img.shields.io/badge/C-A8B9CC.svg?style&logo=C&logoColor=black" alt="C" />
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

The project is a graphical user interface (GUI) for a game called "Chutes and Ladders", implemented in C++ using the Qt framework. It handles functionalities such as creating a game board, allowing players to roll and reroll dice, moving pawns on the board, undoing moves, and displaying leaderboards. The purpose of the project is to provide an interactive and visually appealing interface for playing the game, enhancing the user experience.

---

## ⚙️ Features

| Feature                | Description                                                                                                                         |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| **⚙️ Architecture**     | The codebase follows an object-oriented architecture. It utilizes the Qt framework for GUI components and implements various classes representing game elements like players, pawns, tiles, and the game board.                                                                           |
| **📖 Documentation**   | The codebase lacks detailed documentation. Although some code files have brief comments, the overall documentation is limited. The lack of comprehensive documentation may make it difficult for new contributors to understand and navigate the codebase efficiently.                                                        |
| **🔗 Dependencies**    | The codebase relies on the Qt framework for GUI components and implements various functionalities like random number generation, GUI management, and XML parsing.                                                                          |
| **🧩 Modularity**      | The codebase is organized into several classes that represent different game elements. The classes are modular and aim to provide segregated logic for different functionalities. However, the loose coupling and separation of concerns could be improved to enhance maintainability and reusability.                                                          |
| **✔️ Testing**          | The codebase does not provide specific information on testing strategies and tools. It would be beneficial to have unit tests to validate the functionality and behavior of individual components.                                                                                                                                 |
| **⚡️ Performance**      | The performance of the codebase depends on the efficiency of the Qt framework, which is widely used and known for its optimization. Overall, the codebase doesn't exhibit any glaring performance concerns in terms of speed, efficiency, or resource usage.                                    |
| **🔐 Security**        | The codebase does not have specific security measures mentioned. Given its nature as a GUI-based board game, security concerns may not be a top priority. However, best practices, such as data sanitization, authentication, and secure protocols, should be considered if the application handles sensitive information.           |
| **🔀 Version Control** | The codebase uses Git as its version control system. The repository on GitHub makes it easy to track changes, collaborate with other developers, and manage different versions of the codebase.                                                                  |
| **🔌 Integrations**    | There are no explicit integrations mentioned in the codebase. However, as it relies on the Qt framework, there might be implicit integrations with external libraries such as OpenGL for graphics rendering and other Qt-supported libraries and features.               |
| **📶 Scalability**     | The codebase does not have explicit scalability considerations. Further analysis is required to evaluate whether the system can handle substantial growth, such as supporting a large number of players and expanding game features efficiently. The extensibility of the codebase can significantly impact its scalability. |

---


## 📂 Project Structure




---

## 🧩 Modules

<summary>Root</summary>

| File                                                                                                                 | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ---                                                                                                                  | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [marble.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/marble.cpp)                               | The provided code defines the implementation of a class called Marble, which inherits from QObject. It initializes the Marble object with a given parent and doesn't have any additional functionality.                                                                                                                                                                                                                                                                |
| [leaderboarddialog.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/leaderboarddialog.cpp)         | This code snippet reads data from a CSV file and displays it in a leaderboard format. It calculates win percentages and sorts the statistics accordingly before presenting them on the screen.                                                                                                                                                                                                                                                                         |
| [leaderboarddialog.ui](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/leaderboarddialog.ui)           | This code snippet is an XML file defining a UI for a leaderboard dialog. It describes a QDialog widget with a push button for closing the dialog. The file sets the geometry and window title of the dialog. It doesn't contain any additional resources or connections. Total characters: 335                                                                                                                                                                         |
| [player.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/player.cpp)                               | The provided code snippet defines the functionality for a Player class in a game. The class includes functions to initialize the player, undo moves, roll dice, and reroll dice. It also includes an equality operator to compare players. The code utilizes the Qt framework for random number generation and visual elements.                                                                                                                                        |
| [usernamesdialog.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/usernamesdialog.cpp)             | The code defines a dialog window for entering usernames. It dynamically creates labels and text fields for each player's username. When the start button is clicked, it retrieves the usernames entered and stores them in a vector before closing the dialog.                                                                                                                                                                                                         |
| [tile.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/tile.h)                                       | The code snippet defines a Tile class that inherits from QGraphicsItem. It represents a tile in a graphical interface. Each tile has attributes such as position, width, tile number, whether it has a shortcut, and shortcut number. It also provides functions to get and set these attributes, as well as methods for painting and defining the shape of the tile.                                                                                                  |
| [numplayersdiaglog.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/numplayersdiaglog.h)             | The code snippet defines a dialog box that allows the user to enter the number of players. It inherits from the QDialog class and has a constructor, a destructor, and a function to retrieve the chosen number of players. The dialog includes a submit button that triggers a slot function when clicked. The UI is managed by an instance of the Ui::NumPlayersDialog class.                                                                                        |
| [usernamesdialog.ui](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/usernamesdialog.ui)               | The code snippet is an XML file defining the UI layout for a dialog window called UsernamesDialog. The dialog contains a QPushButton widget named startGameButton, and specifies its size and position. The window also has a title "Enter players" and default size. The XML doesn't include any resources or connections.                                                                                                                                            |
| [numplayersdiaglog.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/numplayersdiaglog.cpp)         | This code snippet defines a dialog box for selecting the number of players. The default number of players is set to 2. The submit button updates the num_players_ variable with the value from a number input box and closes the dialog.                                                                                                                                                                                                                               |
| [pawn.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/pawn.h)                                       | The code snippet defines a "Pawn" class that represents a game pawn on a graphical interface. It inherits from QGraphicsObject and includes functionalities for setting and getting the current tile the pawn is on, retrieving the width of the pawn, and painting the pawn on the graphics scene. The class also defines friend operator overloading for comparing equality between two pawns.                                                                       |
| [numplayersdiaglog.ui](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/numplayersdiaglog.ui)           | The provided code snippet is an XML file defining the UI (user interface) of a dialog window. The dialog window allows the user to enter the number of players and submit their usernames. It includes labels, spin boxes, and a submit button. The window has a fixed size and a title.                                                                                                                                                                               |
| [gamewindow.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/gamewindow.cpp)                       | HTTPStatus Exception: 400                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [player.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/player.h)                                   | The provided code snippet defines a Player class that represents a game player. It includes member variables and methods for managing the player's information, such as username, number of rerolls, number of undos, previous positions, pawn, color, dice result, on-board status, and player number. It also provides functionality for rolling the dice, rerolling the dice, and undoing a move.                                                                   |
| [pawn.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/pawn.cpp)                                   | This code snippet defines a class called "Pawn" which represents a pawn object in a game. It includes functions to set the pawn's current tile, define its bounding rectangle and shape, and paint it on a graphics item.                                                                                                                                                                                                                                              |
| [board.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/board.cpp)                                 | The code snippet defines a class called "Board" that creates a vector of tiles representing a game board. It assigns tile numbers to each tile based on their position on the board. The vector is populated with the tiles in a specific order, starting from row 1 and moving through all rows until row 10. Each row alternates its starting side-left to right for even rows and right to left for odd rows.                                                       |
| [chutesAndLadders.pro.user](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/chutesAndLadders.pro.user) | HTTPStatus Exception: 400                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [gamewindow.ui](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/gamewindow.ui)                         | The provided code snippet is an XML format for creating a graphical user interface (GUI) for a game window. It includes various widgets such as buttons, labels, and graphics views. The code defines the layout, properties, and styles for these widgets. The GUI is designed for a game called "Chutes and Ladders.                                                                                                                                                 |
| [tile.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/tile.cpp)                                   | This code defines the functionality of a Tile class. It includes functions for setting the position, size, and appearance of a tile, as well as operators for comparing tiles.                                                                                                                                                                                                                                                                                         |
| [marble.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/marble.h)                                   | The code snippet defines the Marble class, which inherits from QObject. It has a default constructor and no signals.                                                                                                                                                                                                                                                                                                                                                   |
| [leaderboarddialog.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/leaderboarddialog.h)             | This code defines a class called LeaderboardDialog in C++, which is derived from the QDialog class. It has a constructor, destructor, and a function called ReadFile(). It also has a slot, on_pushButton_clicked(), and a private member variable, total_players_. Additionally, there is a namespace for the User Interface called Ui.                                                                                                                               |
| [board.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/board.h)                                     | The provided code snippet is for the "Board" class, which serves as a QGraphicsScene and represents the game board. It has functions to access and set individual tiles on the board, as well as to generate and retrieve a vector of all the tiles. The underlying board is implemented as a 2D array, and the "Tile" class is assumed to be available elsewhere.                                                                                                     |
| [usernamesdialog.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/usernamesdialog.h)                 | The provided code snippet defines a class called UsernamesDialog that is a QDialog subclass.It has a constructor that takes a QWidget pointer and an integer as arguments, and a destructor.It also has a method called get_usernames() that returns a vector of strings.There is a private slot called on_startGameButton_clicked(), and private members including a Ui::UsernamesDialog pointer, an integer num_players_, and a vector of strings called usernames_. |
| [main.cpp](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/main.cpp)                                   | This code sets up a game window and initializes a seed for random number generation. It then creates an application object, a game window object, shows the window, and starts the application event loop.                                                                                                                                                                                                                                                             |
| [gamewindow.h](https://github.com/richardr1126/ShutesAndLaddersGUI/blob/main/gamewindow.h)                           | The `GameWindow` class is the main window for a game. It manages player information, game state, and various game actions such as starting, ending, rolling dice, moving player, and displaying leaderboards. It also contains helper functions for switching players, checking for a win, making a new game, and resetting the game.                                                                                                                                  |


---

## 🚀 Getting Started

### ✔️ Prerequisites

Before you begin, ensure that you have the following prerequisites installed:
> - `ℹ️ Requirement 1`
> - `ℹ️ Requirement 2`
> - `ℹ️ ...`

### 📦 Installation

1. Clone the ShutesAndLaddersGUI repository:
```sh
git clone https://github.com/richardr1126/ShutesAndLaddersGUI
```

2. Change to the project directory:
```sh
cd ShutesAndLaddersGUI
```

3. Install the dependencies:
```sh
g++ -o myapp main.cpp
```

### 🎮 Using ShutesAndLaddersGUI

```sh
./myapp
```

### 🧪 Running Tests
```sh
Insert test command.
```

---


## 🗺 Roadmap

> - [X] `ℹ️  Task 1: Implement X`
> - [ ] `ℹ️  Task 2: Refactor Y`
> - [ ] `ℹ️ ...`


---

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

---

## 📄 License

This project is licensed under the `ℹ️  INSERT-LICENSE-TYPE` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.

---

## 👏 Acknowledgments

> - `ℹ️  List any resources, contributors, inspiration, etc.`

---
