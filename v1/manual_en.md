---
feature: /v1/img/game_plane.png
---
# TechDebt Game Manual

## Overview
The **TechDebt Game** is a board game designed to enhance understanding and discussion of Technical Debt (TD) by simulating the software development process. Two teams of two players compete within a predefined duration (e.g., 60 minutes) to develop a system, making strategic decisions about software architecture and features.

Players accumulate users (points) by completing tasks. While taking on TD may accelerate progress, it also increases future difficulties, reducing the final score. The team with the most users at the end wins.

![TechDebt Game Board](/v1/img/game_plane.png)

The game [is available as a PDF](ENGameManualDigital.pdf) and requires dice and game pieces. 
 
---

## Game Components

### Game Board
The board represents project progress and module placement. Each team builds a system consisting of three modules (A-C).

### Architecture and Feature Tickets
- To start a module, a **Architecture Ticket** must be completed and placed in the first row.
- After that, **Feature Tickets** can be placed in subsequent rows.
- Feature tickets provide points, represented by users gained.
- Each ticket shows six dice values, with some blocked by red marks.
- Two dice are rolled to "work" on a ticket. If a rolled value is not blocked, one task is completed.
- The number of tasks needed to complete a ticket is shown as empty circles.

![Dependencies Example](/v1/img/dependencies_example.png)

### Technical Debt (TD) Incurrence
- **Conscious TD:** A player can choose to add TD to a blocked dice value, allowing immediate completion of a task if that value is rolled.
- **Unconscious TD:** If a double is rolled, TD is automatically incurred on that number, and two tasks are completed immediately.

### Workstation/TD Repayment Card
- This card marks where completed tickets are placed and helps identify dependencies.
- To **repay TD**, the card is flipped to the repayment side.
- Repayment requires a dedicated turn.
  - Feature tickets: Rolling a 4, 5, or 6 removes TD.
  - Architecture tickets: Only a 5 or 6 can remove TD.
- Repayment represents time spent addressing past decisions instead of progressing.

### TD Dependencies
- Each ticket depends on all previous tickets in the same module.
- If previous tickets have TD, those values become blocked on current tickets.
- Example: If a current ticket allows rolling a 6, but a previous ticket has TD on a 6, it is no longer valid for task completion.

### Event and Action Cards
- **Event Cards (❓)** have immediate negative effects, simulating TD causes and consequences.
- **Action Cards (❗)** can be used strategically to manage TD effectively.

---

## Objective
The game challenges players to balance short-term gains with long-term consequences, promoting discussion on TD management strategies. The winning team is the one that accumulates the most users by the end of the game.
