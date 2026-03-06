# 🚀 RouteMaster Pro - AI Warehouse Optimization

An advanced, interactive web-based warehouse order picker route optimization application using multiple pathfinding algorithms (BFS, A*, Dijkstra).

---

## 📋 Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [How to Use](#how-to-use)
- [Grid Builder](#grid-builder)
- [Algorithms](#algorithms)
- [Output & Visualization](#output--visualization)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Technologies](#technologies)

---

## ✨ Features

### 🔧 Interactive Grid Builder
- **Visual Grid Creation**: Click to place obstacles, targets, and start position
- **Dynamic Sizing**: Customize grid rows and columns (2-20)
- **Three Building Modes**:
  - 🔵 **Start Position**: Set picker starting location
  - 🎯 **Targets**: Add items to collect
  - ⬛ **Obstacles**: Place shelves and walls

### 📊 Multiple Pathfinding Algorithms
- **BFS (Breadth-First Search)**: Finds shortest path by exploring level-by-level
- **A* Algorithm**: Heuristic-based pathfinding for optimized routes
- **Dijkstra's Algorithm**: Guaranteed shortest path with distance tracking

### 🎬 Route Animation
- Real-time path animation with customizable speed
- Live step numbers showing exact path progression
- Target collection detection with sound effects
- Completion status tracking

### 📈 Performance Metrics
- **Calculation Time**: Algorithm execution duration
- **Path Efficiency**: Percentage of grid optimally used
- **Grid Complexity**: Obstacle density percentage

### 🎨 Visualization
- **Color-Coded Grid**:
  - Blue: Start position (S)
  - Orange: Target items (T)
  - Black: Obstacles/Shelves (█)
  - Green: Completed path with step numbers
  - Green Gradient: Current picker position (🤖)
  - White: Walkable areas

### 🎵 Additional Features
- Sound effects toggle
- Light/Dark mode themes
- JSON output export
- Live statistics display
- One-click demo scenario loading

---

## 🚀 Getting Started

### Prerequisites
- Web browser (Chrome, Firefox, Safari, Edge)
- No installation required

### Running Locally

**Option 1: Direct File Opening**
```bash
# Simply open the file in your browser
Double-click Untitled-1.html
```

**Option 2: Local HTTP Server (Recommended)**
```bash
# Navigate to the directory
cd c:\Users\Paavana\Downloads

# Python 3
python -m http.server 8000

# Then open in browser
http://localhost:8000/Untitled-1.html
```

---

## 📖 How to Use

### Step 1: Set Grid Dimensions
1. Enter desired **Grid Rows** (2-20)
2. Enter desired **Grid Columns** (2-20)
3. Grid updates automatically

### Step 2: Build Your Warehouse Layout

**Start Position** (🔵 Start)
- Click the "🔵 Start" button
- Click a cell in the grid builder to set the picker's starting location
- Only one start position allowed

**Add Targets** (🎯 Targets)
- Click the "🎯 Targets" button
- Click multiple cells to mark items that need to be collected
- Click again to remove a target

**Place Obstacles** (⬛ Obstacles)
- Click the "⬛ Obstacles" button
- Click cells to place shelves and walls
- Create a challenging warehouse layout

### Step 3: Select Algorithm
Choose your pathfinding approach:
- 🧠 **BFS Algorithm**: Good for simple grids
- ⭐ **A* Algorithm**: Faster with good heuristics
- 🎯 **Dijkstra**: Most reliable for complex paths

### Step 4: Calculate Route
Click **🎯 Calculate Route** button
- System computes optimal path visiting all targets
- Displays calculation time and efficiency metrics
- Grid shows numbered path steps (0 = start, 1-N = steps)

### Step 5: Watch Animation
1. Click **▶️ Start Route Animation**
2. Adjust speed with slider:
   - 🚀 Very Fast (100-200ms)
   - ⚡ Fast (200-400ms)
   - ⏱ Normal (400-600ms)
   - 🐢 Slow (600-1000ms)
3. Watch picker (🤖) follow the calculated route
4. See real-time step counting and target collection

### Step 6: View Results

**JSON Result Tab**
- Complete path data with coordinates
- Target collection count
- Total steps taken
- Calculation performance metrics
- Copy to clipboard functionality

**Statistics Tab**
- Total steps required
- Targets collected
- Grid dimensions
- Click for detailed hover info

---

## 🔨 Grid Builder Details

### Visual Feedback
- Cells show content: **S** (start), **T** (target), **█** (obstacle)
- Hover over cells for scale effect
- Click to toggle between modes

### Current Mode Display
Shows active building mode at bottom of Grid Builder section

### Grid Limits
- Minimum: 2×2 grid
- Maximum: 20×20 grid
- Recommended: 5×10 to 10×10 for optimal performance

---

## 🧠 Algorithms Explained

### BFS (Breadth-First Search)
- **Time Complexity**: O(rows × cols)
- **Space Complexity**: O(rows × cols)
- **Best For**: Small grids, guaranteed shortest path
- **Speed**: Fast on simple layouts

### A* Algorithm
- **Time Complexity**: O(rows × cols × log(rows × cols))
- **Space Complexity**: O(rows × cols)
- **Heuristic**: Manhattan distance
- **Best For**: Complex mazes, efficient pathfinding
- **Speed**: Faster than Dijkstra with good estimates

### Dijkstra's Algorithm
- **Time Complexity**: O((rows × cols)²)
- **Space Complexity**: O(rows × cols)
- **Best For**: Weighted grids, guaranteed shortest path
- **Speed**: Reliable but slower on large grids

---

## 📊 Output & Visualization

### JSON Result Format
```json
{
  "path": [[0,0], [0,1], [1,1], ...],
  "targets_collected": 4,
  "total_steps": 23,
  "calculationTime": 2.45
}
```

### Performance Metrics
- **Calculation Time**: Milliseconds to compute route
- **Path Efficiency**: Successfully used grid percentage
- **Grid Complexity**: Obstacle density as percentage

### Grid Display
- **Final Output**: Shows complete route with step numbers
- **Animation**: Displays live movement during playback
- **Legend**: Reference for all cell types

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Enter` | Calculate route |
| `Click` | Place/remove grid elements |
| Slider | Adjust animation speed |

---

## 🎨 Theme Options

### Dark Mode (Default)
- Professional dark gradient background
- Blue/purple accent colors
- Optimized for extended use

### Light Mode
- Bright purple gradient background
- Dark accent colors
- High contrast text

Toggle with **🌙 Dark Mode** / **☀️ Light Mode** button

---

## 🔊 Sound & Feedback

### Sound Effects
- ✅ Toggle with **🔊 Sound On** / **🔇 Sound Off**
- **Move Sound**: Lower pitch beep for each step
- **Target Sound**: Higher pitch for collecting items
- **Complete Sound**: Melodic chime on route completion

---

## 📱 Responsive Design

- Optimal on **1400px+ width** (Desktop)
- Single column layout on **<1200px** (Tablets/Mobile)
- Grid rebuilds automatically on resize

---

## 🛠️ Technologies Used

- **HTML5**: Structure and semantics
- **CSS3**: Modern styling with gradients, animations, and transitions
- **Vanilla JavaScript**: No dependencies required
- **Canvas API**: Path visualization (optional)
- **Web Audio API**: Sound effects

---

## 💡 Tips & Best Practices

### For Best Results
1. Start with simpler grids (5×5 or 6×8)
2. Place obstacles to create interesting challenges
3. Use A* or Dijkstra for complex mazes
4. Try different algorithms to compare performance
5. Load demo scenario for quick testing

### Common Scenarios
- **Tight Aisles**: Use Dijkstra for reliability
- **Open Warehouse**: BFS is very fast
- **Mixed Layout**: A* balances speed and efficiency

### Performance Tips
- Large grids (15×15+) may be slower with many obstacles
- Animation speed affects perceived performance
- Multiple targets increase computation time

---

## 📝 Example Workflow

1. Open HTML file in browser
2. Click "📦 Load Demo Scenario" (auto-fills example)
3. Select **⭐ A* Algorithm**
4. Click **🎯 Calculate Route**
5. Click **▶️ Start Route Animation**
6. Watch picker navigate to all targets
7. View JSON result and statistics

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| No path found | Add more walkable cells or move targets closer |
| Slow animation | Increase animation speed slider |
| No sound | Enable with 🔊 button |
| Grid not updating | Refresh page or check row/column values |

---

## 📄 License

Free to use for educational and commercial purposes.

---

## 🙏 Credits

**RouteMaster Pro v1.0** - AI-Powered Warehouse Optimization

Built with pathfinding algorithms and interactive visualization

---

## 🎯 Future Enhancements

- Multi-agent pathfinding
- Weighted grid support
- Custom obstacle shapes
- Route comparison tools
- API integration
- Export route as image/PDF

---

**Happy Route Optimizing! 🚀**

For issues or suggestions, test different grid configurations and algorithms to find optimal solutions for your warehouse layout.
