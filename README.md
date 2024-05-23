# Tic-Tac-Toe Game

This project is a web-based implementation of the classic Tic-Tac-Toe game using Java Servlets and JSP. The game allows two players to take turns placing their respective signs (X or O) on a 3x3 grid.

## Project Overview

The project includes the following key features:

- **Interactive Game Board:** A dynamic 3x3 grid where players can click to place their signs.
- **Game Logic:** Automatic handling of player moves, checking for wins, and determining draws.
- **Session Management:** Each game session is maintained using HTTP sessions to track the state of the game.
- **Reset Functionality:** A feature to restart the game at any time by invalidating the current session.

## Setup and Configuration

### Prerequisites

- Java 1.8 or higher
- Apache Tomcat (version 9 or higher recommended)
- Maven (for building the project)

### Installation

1. **Clone the Repository:** Clone the repository to your local machine.
2. Deploy the application on your Java web server.
3. **Download and Install Tomcat 9:** Follow the official Tomcat documentation for installation instructions.
4. **Configure the Program Launch through IDEA:** Follow the official IntelliJ IDEA documentation for configuration instructions.
5. **Access the Application:** Open your web browser and navigate to: `http://localhost:8080`

## Code Structure

- **Field Class:** Represents the game board with methods for accessing and manipulating the board.
- **InitServlet Class:** Initializes the game by creating a new session, generating a new game board, and redirecting to the main game page.
- **LogicServlet Class:** Handles player moves and game logic, such as checking for a win or a draw.
- **RestartServlet Class:** Resets the game by invalidating the current session and redirecting to the game initialization.
- **Sign Enum:** Represents the possible signs on the game board (EMPTY, CROSS, NOUGHT).
- **index.jsp:** JSP page for rendering the game board and displaying game results.

## How to Play

### Start the Game
Navigate to `http://localhost:your-port/start` to initialize a new game session.

### Make a Move
Click on any cell in the 3x3 grid to place your sign (X). The game will alternate turns between X and O.

### Game Outcome
The game will display a message indicating whether X or O wins or if the game is a draw. You can restart the game at any time by clicking the "Start again" button.

## Built With

- **Java Servlet API:** Used for handling HTTP requests and managing sessions.
- **JavaServer Pages (JSP):** Used for rendering the game interface.
- **jQuery:** Used for asynchronous communication (e.g., restarting the game).
