# Tic-Tac-Toe Game

This repository contains a simple implementation of the classic Tic-Tac-Toe game in Java. The game utilizes Java Servlets for the backend and JSP for the frontend, allowing two players to take turns placing their respective signs (X or O) on a 3x3 grid.

## Getting Started

To run the application, you need a Java web server (e.g., Apache Tomcat) and a web browser. Follow these steps:

1. Clone the repository:
 <pre><code>git clone https://github.com/your-username/tic-tac-toe.git</code></pre>
2. Deploy the application on your Java web server.

3. Access the application in your web browser by navigating to http://localhost:your-port/start.

## Code Structure

- **Field Class:** Represents the game board with methods for accessing and manipulating the board.
- **InitServlet Class:** Initializes the game by creating a new session, generating a new game board, and redirecting to the main game page.
- **LogicServlet Class:** Handles player moves and game logic, such as checking for a win or a draw.
- **RestartServlet Class:** Resets the game by invalidating the current session and redirecting to the game initialization.
- **Sign Enum:** Represents the possible signs on the game board (EMPTY, CROSS, NOUGHT).
- **index.jsp:** JSP page for rendering the game board and displaying game results.

## How to Play

1. Start the game by navigating to http://localhost:your-port/start.

2. Click on the cells of the grid to make your move. Alternatively, restart the game at any time.

3. The game will notify you if there's a winner or if it's a draw. You can restart the game after completion.

Enjoy playing Tic-Tac-Toe!

## Dependencies

- Java Servlet API
- JavaServer Pages (JSP)
- jQuery (for asynchronous restart functionality)

## License

This project is licensed under the MIT License - see the [LICENSE.md] file for details.
