# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-09-27

### Added
- Initial release as Unity Package Manager compatible package
- Track compilation and domain reload times
- Advanced cause detection for recompilation triggers
- History tracking for compile/reload events
- Visual analytics and warnings for long compile times
- Editor window with detailed statistics and tips

### Features
- Real-time tracking of Unity compilation and domain reload times
- Detailed cause analysis for what triggered recompilation
- Historical data with graphs and statistics
- Performance warnings when compile times exceed thresholds
- Productivity tips and optimization suggestions
- Persistent data storage using EditorPrefs

### Technical
- Organized code into proper namespace `GameDevBox.TrackWastedTime.Editor`
- Added assembly definition for proper Unity package structure
- Compatible with Unity 2019.4 and newer versions