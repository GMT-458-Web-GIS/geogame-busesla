[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/BhShQpq1)
# 🌍 Global Dance Locator - GeoGame Assignment 💃🕺

**Student:** [Your Name Surname]
**Course:** Web GIS & Geovisualization (Example)
**Deadline:** 📅 November 17, 2024

---

## 📸 Project Visual Identity

The following image represents the visual identity of the **"Global Dance Locator"** GeoGame. The design effectively blends global map elements with dynamic dancer silhouettes, music notes, and a compass rose, encapsulating the core concept of geographical culture and movement.



---

## 1. Project Overview & Core Components 🗺️

This project is an interactive, time-bound GeoGame developed using standard web technologies (HTML, CSS, JS). The game challenges the user to accurately locate the geographical origins of various global dance types (e.g., Samba, Waltz, Capoeira).

| Component | Focus | Description |
| :--- | :--- | :--- |
| **Geo-Component** | 📍 Map Interaction | Mandatory use of a map to capture user coordinates and calculate distances. |
| **Temporal Component** | ⏱️ Time Constraint | A strict **60-second** limit to complete as many tasks as possible. |
| **Theme** | ✨ Dance Culture | Utilizes a database of world dance styles (Tango, Hula, Flamenco, etc.) and their origins. |

---

## 2. Identify the requirements and the layout of your frontend.

### A. Set of Requirements (Game Logic & Geospatial)

All requirements are structured to ensure both robust game mechanics and accurate geospatial data handling.

| ID | Category | Requirement | Success Metric |
| :--- | :--- | :--- | :--- |
| **R1** | **Map** | Interactive Base Map | Full-screen, navigable map rendered via Leaflet.js. |
| **R2** | **GIS** | Coordinate Capture | `lat/lng` captured on a single user click. |
| **R3** | **GIS** | Distance Calculation | Uses **Haversine Formula** to calculate km distance to the true origin. |
| **R4** | **Feedback** | Visual Marking | Displays distinct markers for **User Guess (🔴)** and **True Origin (🟢)**. |
| **R5** | **Game** | Time Limit | Visible countdown timer (60 seconds max). |
| **R6** | **Game** | Proximity Scoring | Score awarded is inversely proportional to the error distance (closer click = higher score). |
| **R7** | **Game** | Life System | Tracks and manages the user's three allocated lives. |

### B. Frontend Layout Sketches (Structure and Hierarchy)

The user interface adopts a clear, two-column split-screen layout to prioritize the interactive map.

#### 🖥️ Desktop Layout Breakdown

| Section | Size | Content Focus | Emojis |
| :--- | :--- | :--- | :--- |
| **Map Area** | **70%** (Primary) | Leaflet/OpenLayers Map; Click handling; Answer visualization. | 🗺️📍 |
| **Control Panel** | **30%** (Secondary) | Game status, Question prompt, Feedback. | 📊❓ |

---

## 3. Game Progression, Questions, and Lives

| Question | Answer Details | Progression Style |
| :--- | :--- | :--- |
| **How will the game progress?** | The game uses a **Time-Based Race** mechanic. Users complete random tasks against a constant **60-second** clock. | **Progression:** Start $\rightarrow$ New Question $\rightarrow$ User Click $\rightarrow$ Score/Life Update $\rightarrow$ Next Question (Loop until time/lives run out). |
| **How many questions will there be?** | **Unlimited.** The goal is task completion; questions are drawn randomly from a list of 20+ dances. | **Difficulty:** Based on speed and geographical precision. |
| **How many lives does a user have?** | The user starts with **3 Lives** (❤️ ❤️ ❤️). | **Game Over:** 1. Time runs out, OR 2. Lives $\rightarrow$ 0. |

---

## 4. JS Library Planning (Mandatory & Bonus)

| Library | Type | Purpose in GeoGame | Bonus Points 🌟 |
| :--- | :--- | :--- | :--- |
| **Leaflet.js** | Mandatory Geo | Renders the base map, manages map tiles, and handles user click events (R1, R2). | N/A |
| **D3.js** | Advanced (Bonus) | Creates an overlaying **SVG layer** on the map (R4). | ✅ **Yes.** Used to visualize user performance spatially (accuracy heatmap) with dynamic green/red circles. |
| *OpenLayers/Cesium* | *Alternative* | *(Reserved as potential alternatives)* | N/A |
