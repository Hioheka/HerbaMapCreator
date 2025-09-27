# Herba Map Creator v.0.0.1

A powerful, realistic procedural map generator with manual editing capabilities. Generate maps that follow real-world geography rules with rivers that meander, mountains that form realistic peaks, and forests that grow organically.

![Herba Map Creator](https://img.shields.io/badge/version-0.0.1-blue.svg)
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

### Interactive Editor Mode
- **Manual drawing**: Paint directly on the map with mouse/touch support
- **5 Surface types**: Plains (1), Mountains (2), Shallow Water (3), Deep Water (4), Forests (5)
- **Adjustable brush**: 1-5 brush sizes with circular brush pattern
- **Keyboard shortcuts**: Use 1-5 keys for surface types, +/- for brush size
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
   - `1-5`: Switch surface types
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

### Algorithms Used
- **Improved Perlin Noise**: Multi-octave noise for realistic terrain
- **Height-based placement**: All features respect elevation rules
- **River tracing**: Physics-based meandering with momentum and direction
- **Flood fill**: Organic feature growth with natural boundaries
- **Edge smoothing**: Coastal areas naturally transition to sea level
- **Mountain cleanup**: Aggressive isolation removal for realistic peaks

## Installation

### Option 1: Direct Use
Simply download `index.html` and open in any modern browser.

### Option 2: Local Development
```bash
git clone https://github.com/Hioheka/HerbaMapCreator.git
cd herba-map-creator
# Open index.html in browser or serve with local server
```

### Option 3: Web Server
Upload `index.html` to any web server - no backend required!

## Use Cases

- **Game Development**: Generate realistic game world maps
- **D&D Campaigns**: Create fantasy world geography
- **Educational Projects**: Demonstrate geographic principles  
- **World Building**: Design consistent fictional worlds
- **Prototyping**: Quick terrain concepts for larger projects

## Performance Optimizations

- **Deferred code generation**: C# output only generated when requested
- **Real-time canvas updates**: Smooth brush performance
- **Efficient rendering**: Optimized cell size calculation
- **Memory management**: Proper cleanup and garbage collection

## Planned Features (v.0.0.2)

- [ ] Island generation mode
- [ ] Climate zones
- [ ] City/settlement placement
- [ ] Road network generation
- [ ] Biome transitions
- [ ] Export to PNG/SVG
- [ ] Undo/Redo functionality
- [ ] Layer system

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Inspired by real-world geography and hydrology
- Built with vanilla HTML5, CSS3, and JavaScript
- No external dependencies required

## Contact

- Create an [Issue](https://github.com/Hioheka/herba-map-creator/issues) for bug reports
- [Discussions](https://github.com/Hioheka/herba-map-creator/discussions) for feature requests

---

**Made with care for world builders and game developers**