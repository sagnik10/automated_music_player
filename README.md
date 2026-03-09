# Web Music Player

A responsive web-based music player built using HTML, CSS, and JavaScript. The application provides an interactive audio playback interface with animated visuals, a dynamic playlist, and a fully client-side architecture designed to run directly in modern web browsers.

## Overview

This project implements a lightweight browser music player that combines real-time UI updates with HTML5 audio playback. The interface includes visual animations, dynamic track navigation, and responsive layout behavior suitable for both desktop and mobile devices.

The application is implemented as a static front-end project without any backend services or external frameworks, making it suitable for static hosting platforms such as GitHub Pages.

## Features

* HTML5 audio playback
* Play, pause, next, and previous track controls
* Clickable progress bar with seek functionality
* Automatic track progression
* Dynamic playlist sidebar
* Active track highlighting
* Rotating album artwork animation
* Canvas-based animated background
* Floating particle visual effects
* Audio visualizer bars
* Responsive layout for mobile and desktop devices
* Fully client-side implementation

## Technology Stack

| Layer        | Technology                 |
| ------------ | -------------------------- |
| Markup       | HTML5                      |
| Styling      | CSS3                       |
| Logic        | Vanilla JavaScript         |
| Audio Engine | HTML5 Audio API            |
| Animations   | CSS Keyframes + Canvas API |
| Deployment   | GitHub Pages               |

## Application Architecture

The application follows a modular front-end structure composed of several functional components:

### Player Interface

Responsible for rendering the central playback UI, including controls, track information, album artwork, and progress tracking.

### Playlist Controller

Manages track selection, playlist navigation, and synchronization between the interface and the audio playback state.

### Audio Engine

Utilizes the HTML5 Audio API to control playback, track progress, seeking, and automatic track transitions.

### Visual Animation System

Canvas-based rendering is used to create animated visual environments including moving background particles and floating effects. Additional CSS animations provide vinyl rotation and visualizer bar motion.

## File Structure

```
Music_Player
│
├── index.html
├── README.md
├── DebornaImage.jpeg
├── Tum_Hi_Dekho_Na.mp3
├── Jaadu_Hein_Naasha_Hein.mp3
├── Mere_Dholna_Sun.mp3
├── Zara_Sa.mp3
└── Aaro_Ekbar.mp3
```

## Deployment

The project is designed for static hosting environments and can be deployed using GitHub Pages.

Example deployment:

```
https://USERNAME.github.io/music-player
```

## Performance Characteristics

* Fully client-side execution
* No external libraries or frameworks
* Lightweight rendering
* Smooth animations using requestAnimationFrame
* Optimized for modern browsers

## Usage

1. Clone the repository.

```
git clone https://github.com/USERNAME/music-player.git
```

2. Open the project directory.

3. Launch `index.html` in any modern web browser.

## Future Improvements

* Integration with Web Audio API for real spectrum analysis
* Dynamic theme switching
* Playlist persistence using browser storage
* Enhanced visual effects and transitions
* Improved mobile UI controls

## License

This project is released under the MIT License.
