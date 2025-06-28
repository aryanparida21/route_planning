# Route Planning Project 🚗🗺️

This project implements **A\*** search algorithm to find the shortest path between two points on a real OpenStreetMap (OSM) dataset. Built in C++, it uses the **io2d** graphics library to render the computed route visually.

---

## 📸 Preview

![Map Preview](map.png)

---

## 🧰 Features

- Parses and reads OSM data.
- Accepts user input for start and end coordinates.
- Runs A\* search to compute the shortest path.
- Visually renders the result using `io2d`.

---

## 🛠️ Build & Run Instructions

### ✅ 1. Clone with submodules

```bash
git clone --recurse-submodules https://github.com/aryanparida21/route_planning.git
cd route_planning


✅ 2. Create Build Directory

mkdir build && cd build
cmake ..
make -j$(nproc)

✅ 3. Run

./OSM_A_star_search

📥 It will use ../map.osm by default or let you specify your own:

./OSM_A_star_search -f your_map_file.osm

💡 Example Usage

Set start and ending points: start_x start_y end_x end_y
10 10 90 90
Distance: 851.123 meters.

🔧 Dependencies

    cmake >= 3.11.3

    g++ >= 7.4.0

    make

    IO2D graphics library

🧠 Algorithm Used

The core of the pathfinding logic is the A* (A-star) search algorithm, an informed search algorithm using:

f(n) = g(n) + h(n)

Where:

    g(n) = cost from start to node n

    h(n) = heuristic (straight-line) estimate from n to goal

🙋‍♂️ Author

👨‍💻 Aryan Parida
🔗 github.com/aryanparida21
