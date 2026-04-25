# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A 2D space shooter arcade game built with pure HTML5 Canvas. No dependencies required.

## Running the Game

Open `index.html` directly in a browser. No build or server needed.

## Controls

- **Move**: Arrow keys or WASD
- **Shoot**: Spacebar

## Code Architecture

Single-file game (`index.html`) with these main systems:

- **Game Loop**: `gameLoop()` function runs at 60fps via `requestAnimationFrame`
- **Player**: Object with position, movement, shooting cooldowns
- **Enemies**: Array spawned randomly, move downward with sinusoidal horizontal drift
- **Bullets**: Separate arrays for player and enemy bullets
- **Powerups**: Upgrade system with 3 types (double-shot, laser, invincible), each lasting 10 seconds
- **Particles**: Explosion effects using simple physics (velocity + fade)

## Key Game Constants

- Canvas: 800x600 pixels
- Frame rate: ~60fps
- Enemy spawn rate: 0.02 per frame
- Powerup spawn rate: 0.006 per frame
- Powerup duration: 600 frames (10 seconds)

## Making Changes

This is a simple single-HTML project. Edit `index.html` directly. Test by opening the file in a browser.