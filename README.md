🌙 "The Awakening" — Interactive Decision-Based Web Game
A narrative-driven web application built with Java Servlets and JSP. The project immerses the player in a mysterious dreamscape where survival depends on strategic choices. Beyond the gameplay, this project demonstrates robust server-side state management and a comprehensive unit testing suite.

🎮 Game Overview
The player awakens in a dream and must navigate through a series of challenges.

Dynamic Flow: Every "scene" is managed by Servlets that process user decisions via GET/POST requests.

Consequences: Incorrect choices redirect the player to a "failure" state, while correct paths lead toward the "Awakening."

Persistence: The server tracks player statistics (Wins/Losses) globally using a Map<String, int[]> stored within the ServletContext, ensuring data persists during the server's lifecycle.

🧠 Key Technical Features
MVC Pattern: Separation of concerns using JSPs for views and Servlets for controller logic.

State & Session Management: Utilizes HttpSession for individual player progress and ServletContext for global stat tracking.

Modern Stack: Fully compatible with Tomcat 11 and Jakarta EE 10 (Servlets 6.0).

Robust Testing: 100% logic coverage using JUnit 5 and Mockito to simulate the web environment.

Functionality Screenshots Description
*************************************
1.MainGUI: Displays the landing page and the game's initial entry point.

2.Username: Displays the interface for user identification and session startup.

3.FirstLevel: Shows the first decision-making stage and the beginning of the narrative.

4.SecondLevel: Displays the intermediate game level with increased decision complexity.

5.ThirdLevel: Shows the final decision stage leading to the story's conclusion.

6.IfYouLose: Displays the "Game Over" screen and the consequences of an unsuccessful choice.

7.SavedProgressState: Shows the session management system tracking wins and losses per user.

8.IfYouWin: Displays the success screen and the final outcome for surviving the dream.
🧪 Unit Testing Suite
To ensure reliability, the project includes a comprehensive test suite that mocks the Servlet environment using Mockito:

Win/Loss Logic: Validates that victory/defeat counters increment correctly in the global map.

Session Validation: Verifies that unregistered users are automatically redirected to the login screen (nombre.jsp).

Route Protection: Tests that specific decisions correctly trigger redirects to perder.jsp or forward to the next stage in index.jsp.

Mocked Objects: Simulations of HttpServletRequest, HttpServletResponse, HttpSession, and ServletContext.

🚀 Technologies Used
Language: Java 17

Web: Jakarta EE 10 (Servlets 6.0, JSP, JSTL)

Server: Apache Tomcat 11

Testing: JUnit 5, Mockito

Build Tool: Maven
▶️ Installation & Execution
Prerequisites: Ensure Tomcat 11 and JDK 17 are installed.

Build: Generate the .war file using Maven:

Bash
mvn clean package
Deploy: Move the .war file to the webapps folder of your Tomcat directory or run directly from IntelliJ/NetBeans using the "Run on Tomcat" configuration.

Access: Open your browser at:
http://localhost:8080/proyectoKaren3_war/
