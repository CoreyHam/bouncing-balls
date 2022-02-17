# 1. Getting Started

## `HTML`

### Create a canvas for JS to draw the balls on

## `CSS`

### Set overflow to hidden and remove margin to make the display look clean

## `JS`

### Set up canvas

```
SET JS canvas to equal HTML canvas;
SET context to canvas element "2d"

SET canvas width and height to window viewport width and height;
```
### Set up size and color randomizer

```
SET random(min, max)
    return a random number within the min and max


SET randomRGB
  return a random RGB value
```

# 2. Setting up the Ball Object

## `JS`

## Ball Properties Defined
- `x` and `y` (x position and y position)
    - The horizontal and vertical coordanates of the ball when program starts

- `velX` and `velY` (x velocity and y velocity)
    - values that constantly change the x and y position of the ball

- `color`
    - sets each ball's color

- `size`
    - sets each ball's size (in pixels)

```
SET class Ball to
   INIT x position, y position, x velocity, y velocity, color, and size
      SET Ball's x position to initialized x position
      SET Ball's y position to initialized y position
      SET Ball's x velocity to initialized x velocity
      SET Ball's y velocity to initialized y velocity
      SET Ball's color to iniitialized color
      SET Ball's size to initialized size
```

## Drawing the Ball


```
SET function draw to
    run "beginPath" from context
    set "fillStyle" from context to equal the Ball's set color
    use "arc" from context to draw a circle by starting centered from the ball object's x and y position, make the radius of the arc equal to the ball object's size, start the arc at angle 0 then use pi to calculate the diamater of the circle
    run "fill" from context
```