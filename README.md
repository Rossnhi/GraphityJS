# Cartesian JS

**GitHub Repository:** [https://github.com/Rossnhi/Cartesian-JS](https://github.com/Rossnhi/) (Replace with specific repo link)

## Overview
**Cartesian JS** is a custom JavaScript library built to create high-quality, animated, and interactive mathematical visualizations directly in the web browser. Inspired by the aesthetic and educational power of Grant Sanderson’s **Manim** (3Blue1Brown), this library aims to provide a lightweight, web-native alternative for rendering mathematical concepts dynamically.

> **Status: Under Refactoring** > The library is currently undergoing a significant architectural overhaul to improve modularity, performance, and API consistency. Documentation is being updated to reflect these structural changes.

---

## Features

### 1. Coordinate System Mapping
* Seamlessly maps abstract mathematical coordinates to pixel-based HTML5 Canvas/SVG space.
* Supports dynamic scaling and translation of axes for real-time zooming and panning.

### 2. Procedural Mathematical Animations
* Smooth interpolation for transitions between mathematical states (e.g., transforming a function or shifting vector bases).
* Time-based rendering loops for consistent animation playback.



### 3. Interactive Visualization
* Event-driven components that allow users to manipulate mathematical variables through UI inputs and see immediate graphical updates.
* Built-in support for rendering common mathematical primitives: vectors, parametric curves, and geometric shapes.

---

## Why Cartesian JS?
Traditional plotting libraries often focus on static data visualization. Cartesian JS is designed specifically for **mathematical storytelling**, focusing on the "how" and "why" through motion and interaction. 

---

## Project Roadmap
* [x] **Core Engine:** Basic coordinate mapping and primitive rendering.
* [/] **Refactoring (Current Phase):** * Modularizing the rendering engine for better extensibility.
    * Enhancing the animation API for complex sequencing.
    * Optimizing canvas performance for high-frequency updates.
* [ ] **Documentation:** Comprehensive API reference and interactive tutorials.
* [ ] **Manim-like Presets:** Pre-built styles for common algebraic and geometric explanations.

---

## Technical Stack
* **Language:** JavaScript (ES6+)
* [cite_start]**Rendering:** HTML5 Canvas / P5.js [cite: 17, 21]
* **Design Patterns:** Object-Oriented Programming (OOP) for mathematical entities.
