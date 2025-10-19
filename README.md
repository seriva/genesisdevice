## About

A project started in early 2007 inspired by the Elder Scrolls: Oblivion and Skyrim. The goal is/was to create an engine with similar capabilities while in the process creating some basic gameplay elements. I revisit this project every so often adding new features or improving it for nostalgic reasons;) 

## Tech Stack

- **Language**: Pascal/Delphi (Free Pascal Compiler)
- **Graphics**: OpenGL with SDL2 for window management
- **Audio**: OpenAL for 3D sound
- **Physics**: Newton Dynamics
- **Build System**: Lazarus IDE / Free Pascal
- **Platforms**: Linux, Windows

## Features

- **Multi-platform**: Using SDL supporting Linux/Windows
- **OpenGL Rendering**: Advanced rendering system with shaders
- **OpenAL Audio**: 3D sound system
- **Newton Physics**: Physics simulation system
- **Modular Shaders**: Custom shader system
- **Post-processing**: FXAA, SSAO and bloom effects
- **Terrain System**: Multi-layered heightmap based terrain
- **Water Effects**: Reflection, refraction, waves and underwater effects
- **Foliage System**: Grass, trees, bushes, rocks with animations
- **Sky System**: Skydome with clouds and animations
- **Scene Management**: Octree based spatial partitioning
- **Lighting**: Forward lighting for outdoor areas with directional lights and soft shadows
- **Deferred Lighting**: Indoor lighting with spot and point lights with soft shadows
- **Content Formats**: Support for MD5, OBJ and DDS with JSON converters
- **Map Editor**: WIP Editor for building maps (Windows only)
- **HUD System**: JSON based system for in-game HUD

## Project Structure
```
genesisdevice/
├── Source/
│   ├── Engine/          # Core engine modules
│   ├── Demo/            # Demo application
│   └── Libraries/       # Third-party libraries (SDL, OpenGL, OpenAL, Newton, JsonTools)
├── Bin/                 # Compiled binaries and assets
├── Scripts/             # Build and utility scripts
└── LICENSE.md
```

## Quick Start

### Prerequisites
- Free Pascal Compiler (FPC) or Lazarus IDE
- SDL2 development libraries
- OpenAL development libraries
- Newton Dynamics (automatically built by script)

### Linux Setup
Run the dependency installation script:
```bash
chmod +x Scripts/debian-dependancies.sh
sudo ./Scripts/debian-dependancies.sh
```

This script will install:
- SDL2, OpenAL, and MPG123 development libraries
- Build tools (cmake, build-essential)
- Newton Dynamics physics library

### Building
1. Open `Source/Demo/Demo.lpi` in Lazarus IDE
2. Configure build settings for your platform
3. Build the project (F9 or Build menu)

### Running
Execute the compiled binary from the `Bin/` directory:
```bash
./Bin/Demo
```
