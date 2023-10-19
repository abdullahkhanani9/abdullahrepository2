---
toc: true
comments: true
layout: post
title: Plan for Passion Project
description: Build your first Blog.  This will help us communicate results.
type: plans
courses: { compsci: {week: 6} }
---
**Passion Project Plan: Multiplayer Frog Fighting Game aka Frognite**
**Purpose:**
Our collective passion for game development has led us to embark on this project. Drawing from our modest but meaningful experience, we aim to create an engaging multiplayer fighting game that showcases our creativity and technical skills.
**Description:**
The heart of our project lies in crafting a dynamic web-based multiplayer fighting game. Players will have the opportunity to select from an array of unique characters, each boasting distinct attributes influencing gameplay. These attributes, such as damage output and health points, will add depth and strategy to the gaming experience.
**Technical Aspect:**
To ensure seamless accessibility, we will deploy the frontend on GitHub Pages. This platform provides an intuitive and user-friendly interface for players to interact with our game.
**Testing Protocol:**
Our development process hinges on rigorous testing. Weekly feedback loops via Slack and GitHub Utterances will provide valuable insights. Additionally, personal testing will be conducted to validate that the game functions in accordance with our vision.
**Scrum Meetings and Schedule:**
At the onset of each week, we will convene for Scrum meetings. These sessions will serve as a compass, guiding us through our objectives, strategies, and task assignments. By categorizing these plans in the tangibles section of our shared repository, we ensure accessibility, visibility, and accountability for all team members.
**Frontend Repository Components:**
1. **HTML Files:** Define the structure and layout of game pages (e.g., main menu, character selection, gameplay interface).
2. **CSS Files:** Control the visual style, layout, and animations to enhance the gaming experience.
3. **JavaScript Files:** Handle client-side logic for interactions, game mechanics, and backend communication.
4. **Assets Folder:** Store images, icons, audio files, and other media elements used in the game.
5. **Libraries and Frameworks:** Include third-party tools to streamline development (e.g., jQuery, Phaser.js).
**Backend Repository Components:**
1. **Database Management:** Scripts for database creation, table structures, and relationships.
2. **Server-side Logic:** Functions and scripts governing player accounts, game state, and multiplayer interactions.
3. **API Endpoints:** Definition and management of endpoints facilitating data exchange between frontend and backend.
4. **Authentication and Security:** Measures safeguarding user data and interactions.
5. **Game State Management:** Logic for tracking player positions, health, and scores.
6. **Database Connections:** Configurations for interfacing with external databases or services.
7. **Error Handling and Logging:** Mechanisms for monitoring and troubleshooting backend code.
8. **Testing and Debugging Tools:** Scripts and configurations for automated testing, debugging, and monitoring.
**Conclusion:**
Our passion project aims not only to showcase our skills but also to provide an immersive gaming experience for players. Through meticulous planning, transparent communication, and diligent testing, we are committed to delivering a multiplayer fighting game that leaves a lasting impression.
————
Expanded part of what the frontend repo will be for:
1. **HTML Files:** These would define the structure of the game's pages. For example, we would have HTML files for the main menu, character selection screen, and the actual gameplay interface.
2. **CSS Files:** These would control the visual style of our game. This includes things like color schemes, fonts, layout, and any animations or transitions we’d want to implement.
3. **JavaScript Files:** This is where the “client-side” logic for your game would reside. It would handle interactions like selecting characters, managing game mechanics (like combat), and communicating with the backend (if needed).
4. **Assets Folder:** This would contain all the visual elements needed for our game, such as character sprites, background images, icons for buttons, and any other media files.
5. **Libraries and Frameworks:** If we choose to use any third-party libraries or frameworks to enhance the development process (e.g., for animations or user interface components), they would be included here.
6. **Testing Files:** If we decide to implement automated testing for your frontend code, these files would be stored in this section of the repository.
7. **Documentation:** We might include user guides for navigating the game's interface, developer documentation to explain the frontend code structure, and any other relevant information for working with the frontend code.
8. **Configuration Files:** These would include any setup files necessary for development tools, build processes, or package management that pertain specifically to the frontend of our game.
9. **Error Handling and Debugging:** Files related to handling errors and implementing debugging tools would be essential for identifying and resolving issues in the frontend code.
In summary, the frontend repository is where the visual and interactive elements of our multiplayer fighting game come to life. It's where the user interface is defined, styled, and programmed to respond to player actions, making it a crucial part of our overall project.
Expanded part of backend repo:
1. **Database Management:** This is where we’ll likely have files related to setting up and managing the database for our game. This could include scripts for creating tables, defining relationships, and handling data storage.
2. **Server-side Logic:** The backend repository would contain files that handle server-side logic. This includes functions and scripts responsible for tasks like managing player accounts, handling game state, and facilitating multiplayer interactions.
3. **API Endpoints:** This is where we’d define and manage those API endpoints. They serve as the bridge for data exchange between the frontend and backend.
4. **Authentication and Security:** Files related to user authentication, authorization, and security measures would be included. This ensures that user data and interactions are protected.
5. **Game State Management:** This would involve files responsible for maintaining the current state of the game, including player positions, health, scores, and other relevant information.
6. **Database Connections:** If your backend interacts with an external database or other services, configurations and connections would be stored in this section.
7. **Error Handling and Logging:** Files related to error handling and logging mechanisms to monitor and troubleshoot issues within the backend code.
8. **Testing and Debugging Tools:** This section could include scripts and configurations for automated testing, as well as tools for debugging and monitoring the backend code.
9. **Documentation:** Just like the frontend repository, we’d want to include documentation specific to the backend. This could involve explanations of database structure, API endpoints, and any other critical information for understanding and working with the backend code.
10. **Deployment and Hosting Information:** We might include files related to deploying the backend on a server or cloud platform.
Overall, the backend repository serves as the engine that powers your multiplayer fighting game. It manages the data, logic, and communication necessary to create a seamless gaming experience for our users. It's a pivotal part of our project's architecture and requires careful planning and organization.
## Design so far
![]({{site.baseurl}}/images/frog-game.jpg)