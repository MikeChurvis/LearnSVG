# SVG Commands

## Line Commands

Below are the five commands that apply to `<path>` nodes.

### Move To

Moves the cursor to the following point.

Syntax:

- `M x y`: move the cursor to the given absolute coordinate.
- `m dx dy`: move the cursor to a new position offset by the given coordinate. Note the change in case: this form requires a lowercase `m`.

### Draw Line

Draws a line from the cursor's current position to the following point.

Syntax:

- `L x y`: draw a line to an absolute coordinate.
- `l dx dy`: draw a line to a relative coordinate. Again, note the difference in case.

### Draw Horizontal Line

Syntax:

- `H x`: line to absolute x value.
- `h dx`: line to relative x value.

### Draw Vertical Line

Syntax:

- `V y`: line to absolute y value.
- `v dy`: line to relative y value.

### Close Path

Terminates a path by drawing a straight line from the current position to the first point of the path.

Syntax:

- `Z`: closes the path.
- `z`: same thing. This command is not case-sensitive.

## Curve Commands

### Cubic Curve

Creates a bezier curve with two control points.

Syntax:

- `C x1 y1, x2 y2, x y`: `x1 y1, x2 y2` are control points. Think of them like handles. `x y` is where the curve ends.
- `c dx1 ... dy`: As above, but relative.
