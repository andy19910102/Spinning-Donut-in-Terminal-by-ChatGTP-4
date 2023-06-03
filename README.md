# Spinning Donut in Terminal by ChatGTP-4

![](https://i.giphy.com/media/YyckGhKjemiangSemu/giphy.webp)

This project is a simple Python script that renders a spinning donut shape in the terminal using ASCII characters. It's an interesting implementation of a console-based animation and demonstrates how we can create visually appealing effects using simple text characters.

This project was designed with the help of OpenAI's language model, ChatGPT-4.

## Features

- Renders a spinning donut shape in the terminal.
- Customizable parameters for the spinning donut, including size, rotation speed, and frame delay.
- Uses NumPy for efficient array manipulations and mathematical operations.

## How to Run

Simply clone this repository to your local machine and run the `spinning_donut.py` file in your Python environment. The donut should start spinning in your terminal!

```bash
git clone https://github.com/username/spinning_donut.git
cd spinning_donut
python spinning_donut.py
```

## Code Overview

The main functionality of this project is encapsulated within the   `SpinningDonut` class in the `spinning_donut.py` file. This class handles initializing the parameters of the donut, computing the frame to render, and displaying the frame in the console. It uses a rotation matrix to rotate the points on the donut, and uses an illumination string to give the illusion of a light source.

Here are the main components of the `SpinningDonut` class:

- `__init__()`: Initializes the parameters of the donut. These include screen size, theta and phi spacing for the rotations, and delay for the animation.

- `get_render_frame()`: Computes the frame to render. It calculates the x, y, z coordinates of each point on the donut after rotation, determines the illumination of each point based on its z-coordinate, and populates the frame with the corresponding characters from the illumination string.

- `render()`: Displays the frame in the console. It clears the console before printing each frame to give the illusion of animation.

- `run()`: Begins the animation. It continuously updates the rotation angles, computes the new frame, and renders it.

- `save_frames_to_json()`: Generates a given number of frames, and saves them as a JSON file. Each frame is converted to a single string, with "\n" as the line separator. The resulting list of frames is then written to a JSON file with the specified filename.

## Contribute

If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

## License

The code in this project is licensed under the MIT license.
