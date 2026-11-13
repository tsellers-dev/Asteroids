# Asteroids

A classic 2D Asteroids arcade game built in Python using [Pygame](https://pygame.org "Pygame official website"), created as part of the [Boot.dev](https://www.boot.dev/ "Boot.dev platform") curriculum.

## Features

- **Player Ship Controls:** Smooth rotation, forward/reverse thrust, and rate-limited shooting.
- **Asteroid Splitting:** Large and medium asteroids split into smaller, faster fragments when destroyed.
- **Collision Detection:** Circle-based hitbox detection between shots, asteroids, and the player ship.
- **Object-Oriented Design:** Modular architecture separating game entities, constants, and the main game loop.

## Project Structure

```text
asteroids/
├── main.py             # Entry point and main game loop
├── player.py           # Player ship movement, rendering, and shooting
├── asteroid.py         # Asteroid behavior, movement, and splitting logic
├── asteroidfield.py    # Spawns asteroids at random screen edges
├── shot.py             # Projectile logic and rendering
├── circleshape.py      # Base class for circular game objects and collision checks
├── constants.py        # Screen dimensions, speeds, radii, and game settings
├── pyproject.toml      # Project dependencies (if using uv)
└── README.md           # Project documentation
```

## Prerequisites

- **Python 3.10+**
- **[uv](https://astral.sh "uv Python package manager")** (recommended, per Boot.dev setup) or **pip**

## Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd asteroids
   ```

2. **Install dependencies:**

   *Using `uv` (Boot.dev default):*
   ```bash
   uv sync
   ```

   *Or using standard `venv` and `pip`:*
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install pygame
   ```

## How to Run

Start the game from the root directory:

*Using `uv`:*
```bash
uv run main.py
```

*Or using Python directly:*
```bash
python3 main.py
```

## Controls

| Key | Action |
| :--- | :--- |
| **W** | Move Forward |
| **S** | Move Backward |
| **A** | Rotate Left |
| **D** | Rotate Right |
| **Space** | Fire Weapon |

## Acknowledgments

- Built following the **Build Asteroids using Python and Pygame** guided project on [Boot.dev](https://www.boot.dev/ "Boot.dev platform").
