# ♟ Fog of War Chess Board Viewer

A visualizer for **Fog of War Chess** that displays the chessboard from FEN strings received via WebSocket messages during live games.

## 📋 How to Use (Step by Step)

### Step 1: Open the Viewer

1. Open this link: **[https://bad-plamen.github.io/fog-of-war-chess-viewer/](https://bad-plamen.github.io/fog-of-war-chess-viewer/)**

### Step 2: Find the FEN in Your Game

1. Open your **Fog of War Chess** game in the browser
2. Press **F12** (or **Ctrl+Shift+I**) to open **Developer Tools**
3. Go to the **Network** tab
4. In the filter box, type: **WS** (to show only WebSocket connections)
5. Click on the WebSocket connection (usually there is only one)
6. Go to the **Messages** tab
7. Look for a message containing **`"mutation":"update_live_game"`**
8. Click on it and copy the **entire message text** (Ctrl+A, Ctrl+C)

### Step 3: Display the Board

1. Go back to the viewer page
2. Paste the copied text into the text box
3. Click **"SHOW BOARD"**

## 🎮 What is Fog of War Chess?

**Fog of War Chess** is a two-player chess variant where:

- Each player can only see their **own pieces** and the squares they attack
- The opponent's pieces are **hidden** (in "fog") until you make contact with them
- This adds an element of **strategy and surprise** – you must predict your opponent's moves without knowing their exact position

## 🎨 Viewer Features

- **Your pieces (White)**: ♙♖♘♗♕♔ (white color with black shadow)
- **Opponent's pieces (Black)**: ♟♜♞♝♛♚ (black color with white shadow)
- **Board**: Standard chessboard with alternating light and dark squares
- **Statistics**: Shows the number of squares and pieces for each player

## 🛠 Local Installation

If you want to run the viewer locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/bad-plamen/fog-of-war-chess-viewer.git