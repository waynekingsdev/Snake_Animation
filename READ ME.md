# Snake Animation

A mouse-following snake animation built with Python and Pygame. Move your cursor inside the window to guide a glowing blue snake.

## Features

- A 25-segment snake that follows your mouse.
- A tapered body with a distinct dark blue head and cyan outlines.
- Movement that stops at the cursor without overshooting.
- A 1200 × 600 window with a dark background.
- Animation capped at 60 frames per second.

## Requirements

- Python 3
- Pygame

## Setup


```powershell
python.exe -m pip install pygame
```


## Run

From the project folder, run:

```powershell
python.exe main.py
```

Move the mouse inside the window to steer the snake. Click the window's close button to exit.

## Customize

Edit these values in `main.py` to change the animation:

| Setting | Default | Purpose |
| --- | --- | --- |
| `WIDTH`, `HEIGHT` | `1200`, `600` | Window dimensions in pixels |
| `segments` | `25` | Number of body segments |
| `spacing` | `15` | Maximum distance between adjacent segment centers |
| `speed` | `8` | Maximum head movement in pixels per frame |
| `BG` | `(5, 5, 20)` | Background color |
| `HEAD_COLOR` | `(0, 25, 180)` | Head color |
| `BODY_COLOR` | `(0, 180, 255)` | Body color |
| `GLOW` | `(0, 255, 255)` | Outer circle color |

Colors use RGB values from 0 to 255. The frame-rate cap is set by `clock.tick(60)`; movement speed is measured per frame, so the animation slows down if the actual frame rate drops.

## Troubleshooting

If you see `ModuleNotFoundError: No module named 'pygame'`, install Pygame with the same interpreter used to run the script:


```
python.exe -m pip install pygame
