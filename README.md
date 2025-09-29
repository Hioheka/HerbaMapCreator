# Herba Map Creator v.0.0.3

A powerful, realistic procedural map generator with manual editing capabilities. Generate maps that follow real-world geography rules with rivers that meander, mountains that form realistic peaks, and forests that grow organically.

![Herba Map Creator](https://img.shields.io/badge/version-0.0.3-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## Features

### Realistic Geography Generation
- **Height-based terrain**: Uses improved Perlin noise for realistic elevation maps
- **Meandering rivers**: Rivers flow naturally from high to low elevations with physics-based curves and momentum
- **Compact mountain peaks**: Mountains form only at highest elevations (75%+ height threshold)
- **Organic forests**: Forests grow in suitable climates and elevations using queue-based spreading
- **Natural coastlines**: Irregular, organic-looking coastlines with proper shallow/deep water transitions
- **Beach and desert generation**: Realistic sand placement along coastlines and in arid inland regions

### Interactive Editor Mode
- **Manual drawing**: Paint directly on the map with mouse/touch support
- **6 Surface types**: Plains (1), Mountains (2), Shallow Water (3), Deep Water (4), Forests (5), Sand (6)
- **Adjustable brush**: 1-5 brush sizes with circular brush pattern
- **Keyboard shortcuts**: Use 1-6 keys for surface types, +/- for brush size
- **Performance optimized**: Real-time drawing with deferred code generation

### Developer-Friendly Output
- **C# Entity Framework**: Direct seed data generation for .NET projects
- **JSON format**: Standard JSON output for any platform
- **One-click copy**: Copy generated code directly to clipboard
- **Customizable dimensions**: 10x10 to 200x200 maps supported
- **Optimized performance**: Code generation only when requested

## Live Demo

[Try Herba Map Creator](https://hioheka.github.io/HerbaMapCreator)

## How to Use

### Automatic Generation
1. Set your desired map dimensions (default 100x100)
2. Click "Generate Map"
3. Your realistic map will be generated automatically

### Manual Editing
1. Generate a base map or start fresh
2. Click "Editor Mode"
3. Select a surface type from the colored buttons
4. Paint on the map with your mouse
5. Use keyboard shortcuts for faster editing:
   - `1-6`: Switch surface types
   - `+/-`: Adjust brush size

### Export Your Map
1. Click "Update Code" to generate current map data
2. Click "Copy C# Code" to copy Entity Framework seed data
3. Paste directly into your .NET project
4. JSON format is also available below the C# code

## Technical Details

### Surface Types
- **1 - Plains (Light Green)**: Basic terrain, most common
- **2 - Mountains (Gray)**: High elevation rocky terrain
- **3 - Shallow Water (Blue)**: Rivers, lakes, coastal areas
- **4 - Deep Water (Dark Blue)**: Oceans, deep lakes
- **5 - Forests (Dark Green)**: Wooded areas at suitable elevations
- **6 - Sand (Sandy Brown)**: Beaches along coastlines and desert regions inland

### Algorithms Used
- **Improved Perlin Noise**: Multi-octave noise for realistic terrain
- **Height-based placement**: All features respect elevation rules
- **River tracing**: Physics-based meandering with momentum and direction
- **Flood fill**: Organic feature growth with natural boundaries
- **Edge smoothing**: Coastal areas naturally transition to sea level
- **Mountain cleanup**: Aggressive isolation removal for realistic peaks
- **Beach generation**: Automatic sand placement adjacent to shallow water
- **Desert formation**: Inland sandy regions far from water sources

## Installation

### Option 1: Direct Use
Simply download `index.html` and open in any modern browser.

### Option 2: Local Development
```bash
git clone https://github.com/Hioheka/HerbaMapCreator.git
cd herba-map-creator
# Open index.html in browser or serve with local server