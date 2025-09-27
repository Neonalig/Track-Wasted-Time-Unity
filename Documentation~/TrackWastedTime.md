# Track Wasted Time Package Documentation

## Overview
Track Wasted Time is a Unity Editor tool that monitors and analyzes compilation and domain reload times to help developers identify performance bottlenecks in their workflow.

## Getting Started

### Installation
1. Open Unity Package Manager (`Window > Package Manager`)
2. Click the `+` button and select `Add package from git URL...`
3. Enter: `https://github.com/GameDevBox/Track-Wasted-Time-Unity.git`
4. Click `Add`

### Usage
1. After installation, go to `Window > Timer Wasted Stats` to open the tracking window
2. The tool automatically starts tracking compilation and domain reload times
3. View statistics, history, and optimization tips in the editor window

## Features

### Real-time Tracking
- Monitors Unity compilation times
- Tracks domain reload durations
- Provides immediate feedback on performance

### Advanced Cause Detection
- Identifies what triggered each recompilation
- Categorizes causes (script changes, asset imports, etc.)
- Helps pinpoint performance bottlenecks

### Historical Analytics
- Maintains history of all compile/reload events
- Shows trends over time
- Calculates averages and statistics

### Performance Warnings
- Alerts when compile times exceed thresholds
- Provides visual indicators for long operations
- Helps maintain development efficiency

### Optimization Tips
- Suggests improvements based on detected issues
- Provides actionable recommendations
- Helps optimize development workflow

## API Reference

### Core Classes

#### `TimeWasterTracker`
Main tracking class that monitors compilation and domain reload events.

#### `TimeWasterWindow`
Editor window that displays statistics and analytics.

#### `TimeWasterHistory` 
Manages historical data storage and retrieval.

#### `RecompileDetector`
Detects and categorizes recompilation causes.

#### `AdvancedCauseDetector`
Advanced analysis of domain reload triggers.

### Enums

#### `RecompileCause`
- `Unknown`: Cause could not be determined
- `ScriptChange`: Script file was modified
- `AssetImport`: Asset was imported
- `AssemblyDefinitionChange`: Assembly definition was modified
- `ProjectSettingsChange`: Project settings were changed

#### `DomainReloadCause`
- `Unknown`: Cause could not be determined
- `EnteringPlayMode`: Entering play mode
- `ExitingPlayMode`: Exiting play mode
- `ScriptRecompilation`: Scripts were recompiled
- `AssetDatabaseRefresh`: Asset database was refreshed

## Configuration

The tool uses Unity's `EditorPrefs` to store configuration and historical data. No additional setup is required.

## Troubleshooting

### Tool Not Appearing in Window Menu
- Ensure the package is properly installed
- Restart Unity if necessary
- Check Console for any error messages

### Data Not Persisting
- Data is stored in `EditorPrefs` and should persist automatically
- If data is lost, it may indicate an issue with Unity's preferences storage

## Support

For issues, questions, or feature requests:
- Watch the tutorial: https://youtu.be/uzLRBZmpw-w
- Visit the GitHub repository: https://github.com/GameDevBox/Track-Wasted-Time-Unity
- Follow @GameDevBox on YouTube for more tutorials