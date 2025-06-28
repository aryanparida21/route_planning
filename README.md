# 🚗 Route Planning Project – A* Pathfinding

This project finds the shortest route between two points on a real map using the A* search algorithm. It reads OpenStreetMap data and renders the result using the `io2d` graphics library.

---

## 📦 Features

- A* search implementation in C++
- Parses and renders real `.osm` map data
- Live user input for start/end coordinates
- Visualizes the path using `io2d`

---

## 🧱 Project Structure

route-planning/
├── src/
│ ├── main.cpp # User input + program entry point
│ ├── route_model.cpp # Map model with helper functions
│ ├── route_planner.cpp # A* pathfinding algorithm
│ ├── render.cpp # Rendering the route
├── map.osm # Map file
├── CMakeLists.txt
└── README.md


---

## 🛠️ Build Instructions

```bash
git clone --recurse-submodules https://github.com/aryanparida21/route_planning.git
cd route_planning
mkdir build && cd build
cmake ..
make -j$(nproc)

🚀 Run the Program

./OSM_A_star_search

You’ll be prompted to enter coordinates:

Set start and ending points: start_x start_y end_x end_y

🔍 How A* Search Works

A* uses:

    g(n): cost from start to current node

    h(n): estimated cost to goal (heuristic)

    f(n) = g(n) + h(n)

It explores paths with the lowest f(n) first, ensuring optimal and fast routefinding.
👤 Author

Aryan Parida
GitHub: @aryanparida21
