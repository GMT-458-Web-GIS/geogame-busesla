[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/BhShQpq1)
# 🌍 Global Dance Locator - GeoGame Assignment

**Course:** GIS Applications and Web Technologies (Example)
**Student:** [Your Name Surname]
**Date:** November 17, 2024 (Submission Deadline)

---

## 1. Project Description and Purpose

This project is an interactive map-based quiz game (GeoGame) titled **"Global Dance Locator,"** developed using HTML, CSS, and JavaScript technologies. The main goal of the game is to measure the user's ability to quickly and accurately identify the geographical origins of various global dance types (Tango, Samba, Flamenco, etc.) on a map.

* **Geo-Component (GIS Component):** The game is built around map interaction (clicking, coordinate calculation).
* **Temporal Component (Time Component):** The user's score is determined within a limited time constraint of 60 seconds.

---

## 2. Requirements

The fundamental technical and functional requirements for the game to operate successfully and provide an interactive user experience are as follows:

| Category | Requirement | Description |
| :--- | :--- | :--- |
| **Map & GIS** | R1: Map View | A global, interactive, and navigable map (Leaflet) must be displayed. |
| | R2: Coordinate Detection | The coordinates of the user's click on the map must be accurately captured. |
| | R3: Distance Calculation | The Haversine formula must be used to calculate the distance (in km) between the clicked point and the actual geographical location of the target dance. |
| | R4: Visual Feedback | Upon answering, the user's guess and the correct location must be marked on the map. |
| **Game Mechanics** | R5: Race Against Time | The game must have a strict 60-second time limit. |
| | R6: Scoring | Close guesses should yield high scores, while distant guesses should result in low/zero scores. |
| | R7: Life System | The user must start with 3 lives (error allowances). |
| **User Interface** | R8: Status Display | Score, Remaining Time, and Remaining Lives information must always be visible. |
| | R9: Question Area | The current dance question must be displayed clearly and in large font. |

---

## 3. Frontend Layout Sketches

The game interface is designed to prioritize map interaction. In desktop view, the screen is vertically divided into two main sections: **Map (70%)** and **Control Panel (30%)**.

### Sketch 1: General Structure

The drawing below represents the main interface layout of the project:
