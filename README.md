# Travel Planner

A C++ program that finds the shortest, fastest, and most cost-effective travel routes between cities using Dijkstra's, Bellman-Ford, and Floyd-Warshall algorithms.

## Features
- Supports three modes of transport: **Aeroplane, Bus, Train**
- Uses **Dijkstra's Algorithm** for shortest distance
- Uses **Bellman-Ford Algorithm** for least travel time
- Uses **Floyd-Warshall Algorithm** for lowest cost
- Reads city and transport data from external files

## Requirements
- C++ Compiler (G++ recommended)
- Standard C++ Libraries
- Input data files (`data_plane.txt`, `data_bus.txt`, `graph.txt`)

## Installation & Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/travel-planner.git
   cd travel-planner
   ```
2. Ensure you have a C++ compiler installed (e.g., g++ for Linux/macOS, MinGW for Windows).
3. Place the required data files (`data_plane.txt`, `data_bus.txt`, `graph.txt`) in the project directory.

## Compilation & Execution
Compile the program using:
```bash
 g++ travel_planner.cpp -o travel_planner
```
Run the program:
```bash
 ./travel_planner
```

## Usage
1. Enter the mode of transport (**AEROPLANE, BUS, or TRAIN**).
2. Input the starting and destination cities.
3. The program will display:
   - **Shortest distance (Dijkstra’s Algorithm)**
   - **Least travel time (Bellman-Ford Algorithm)**
   - **Lowest cost (Floyd-Warshall Algorithm)**
4. If no path exists, the program will notify the user.

## File Format
Each transport mode's data file must contain:
1. **List of cities** (10 cities, one per line).
2. **Three adjacency matrices** (for distance, time, and cost) where `INF` represents no direct connection.

Example (`graph.txt`):
```
CityA CityB CityC ... CityJ
0 10 INF ... 20
10 0 15 ... INF
INF 15 0 ... 25
...
```

## Future Improvements
- Extend the number of cities beyond 10.
- Implement a graphical user interface.
- Support dynamic file input.

## License
This project is open-source under the [MIT License](LICENSE).

## Author
[Redhwan Ahmed Zisan](https://github.com/TheAhmedEffect)

