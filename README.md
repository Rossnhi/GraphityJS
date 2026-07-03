# Graphity

> **A JavaScript library for animated mathematical visualizations.**

Graphity is a lightweight JavaScript library for creating beautiful, interactive and animated mathematical visualizations.

Designed for education, demonstrations, and interactive mathematics, Graphity makes it easy to animate Cartesian planes, function plots, parametric curves, transformations, vectors, and geometric objects while providing built-in interactive primitives for creating engaging visual explanations.
Checkout the [website](https://rossnhi.github.io/Graphity-Site) for more details.
---

## Features

* Interactive Cartesian coordinate system
* Function plotting
* Parametric curves
* Animated points and plot points
* Camera pan and zoom
* Linear transformations
* Customizable grid and viewport
* Lightweight API
* Built on p5.js

---

## Installation

Download the latest `graphity.js` from this repository and include it in your project together with p5.js.

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.11.10/p5.min.js"></script>
<script src="graphity.js"></script>
```

---

## Creating Your First Graph

Create a container for the graph.

```html
<div id="graph"></div>
```

Then create a new Graphity instance.

```javascript
const graph = new Graphity({
    parent: "graph"
});
```

The `parent` option accepts either an HTML element or the ID of an element where the Graphity canvas will be attached.

---

## Basic Usage

### Create a Point

```javascript
const point = graph.addPoint([1, 2]);
```

### Plot a Function

```javascript
const parabola = graph.addPlot(x => x * x);
```

### Plot a Parametric Curve

```javascript
const circle = graph.addParametricPlot(
    [0, 2 * Math.PI],
    t => [
        2 * Math.cos(t),
        2 * Math.sin(t)
    ]
);
```

### Animate

```javascript
graph.draw(() => {

    graph.zoomToCenter();

    graph.panTo([2, 1]);

});
```

Animations return `Animation` objects, allowing complex mathematical animations to be chained together using `.then()`.

```javascript
graph.draw(() => {

    graph.zoomToCenter()
        .then(() => {
            graph.panTo([2, 2]);
        });

});
```

---

## Current Capabilities

Graphity currently supports:

* Cartesian coordinate systems
* Function plots
* Parametric plots
* Interactive points
* Plot points
* Camera zoom
* Camera pan
* Linear transformations
* Grid animations
* Mathematical utility functions
* Continued fractions
* Rational approximation

Copyright (c) 2023 S Roshini
