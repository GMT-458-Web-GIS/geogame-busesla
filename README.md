# 🌍 Global Dance Locator - GeoGame Assignment 💃🕺✨

**Buse Sıla Dolu** 


---

## 📸 Blending Culture & Coordinates

The following image captures the essence of the **"Global Dance Locator"** GeoGame. It represents the successful fusion of dynamic dance culture (silhouettes, music notes) with essential geospatial tools (compass, map coordinates).


<img width="420" height="321" alt="globaldancelocator" src="https://github.com/user-attachments/assets/6e1e7162-1e83-4c1c-b704-c682ebd8ec86" />



---

## 1. Project Mission: The Geo-Dance Challenge 🎯

This is an interactive, time-bound GeoGame developed using HTML, CSS, and JS. The user is challenged to rapidly and accurately locate the geographical origin of various global dance forms (e.g., *Tango*, *Samba*, *Flamenco*) on a world map.

> ⏱️ **Core Principle:** Maximize your score within a **strict 60-second** time limit while managing your limited lives.

---

## 2. Frontend Design: Layout & Requirements

### 📍 Design Philosophy: Map First

My design prioritizes the map interaction. The screen is strategically split to give the user the largest possible canvas for their geospatial guesses.

* **🗺️ Map Area (70%):** The primary workspace. This is where the Leaflet map resides, handling all user clicks and displaying visual feedback (correct/incorrect markers).
* **📊 Control Panel (30%):** The information hub. Dedicated to showing real-time game status and the current question.

#### 📋 Set of Requirements

| Category | ID | Key Functionality | GIS/Game Integration |
| :--- | :--- | :--- | :--- |
| **Map & GIS** | **R1-R4** | **Precision Core** | Uses Leaflet for rendering (R1), captures exact `lat/lng` (R2), and calculates score using the **Haversine Formula** (R3) for distance accuracy. |
| **Game Logic** | **R5-R7** | **Challenge Core** | Enforces the 60-second timer (R5), implements Proximity Scoring (R6), and manages the **3-Life system** (R7). |
| **UI/UX** | **R8-R9** | **User Experience** | Provides constant visibility for Score, Time, and Lives (R8), with a clear, large display for the current question (R9). |

---

## 3. Game Flow & Mechanics 🕹️

### How the game will progress?

* **Style:** **Time-Based Progression** (1-minute sprint).
* **Difficulty:** **Dynamic.** The challenge is the constant time pressure and the need for quick, precise geographical memory. The difficulty level is defined by the proximity threshold for scoring points.
* **Flow:** The timer starts $\rightarrow$ A dance name appears $\rightarrow$ Player clicks $\rightarrow$ Feedback is given $\rightarrow$ New question immediately loads.

### How many questions will there be?

* **Number:** **Unlimited** (Drawn randomly from a curated list of 20+ dances).
* **Goal:** Complete as many tasks as possible before the timer runs out.

### How many lives, if any, does a user have?

* **Lives:** The user starts with **3 Lives** (❤️ ❤️ ❤️).
* **Game Over Condition:**
    1.  ❌ The 60-second timer hits zero.
    2.  ❌ The user's lives count drops to zero.
       
<img width="610" height="656" alt="scheme" src="https://github.com/user-attachments/assets/3b2185af-3dd4-477e-bd02-6f53579af41e" />

---

## 4. JavaScript Library Selection: Powering the GeoGame 💻

I'm utilizing a mandatory map library combined with an advanced package to achieve the bonus scoring criteria.

### 🗺️ Mandatory Geospatial Library

* **Library:** **Leaflet.js**
* **Role:** Provides the lightweight, performant map base and all necessary tools for capturing the coordinates clicked by the user.

### 🌟 Advanced Visualization Package (Bonus Feature)

* **Library:** **D3.js** (Data-Driven Documents)
* **Implementation for Bonus:** D3.js will create a dynamic **SVG performance layer** overlaid on the Leaflet map. This layer will visualize the player's accuracy spatially, acting as a live heatmap:
    * **High Accuracy:** Clicks are visualized as **large, bright green (🟢)** circles.
    * **Low Accuracy/Misses:** Clicks are visualized as **large, red (🔴)** circles, providing compelling visual data analysis of geographical blind spots.
