# Flappy Bird NEAT

This project is an implementation of the Flappy Bird game using the NEAT (NeuroEvolution of Augmenting Topologies) algorithm to train a neural network to play the game.

## Table of Contents

- [Introduction](#introduction)
- [Files](#files)
- [Requirements](#requirements)
- [How to Run](#how-to-run)
- [Configuration](#configuration)
- [Game Logic](#game-logic)
- [NEAT Implementation](#neat-implementation)
- [How to Contribute](#how-to-contribute)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction

This project leverages the NEAT algorithm to train an AI to play Flappy Bird. NEAT evolves neural networks using principles of natural selection, enabling the bird to learn how to navigate through pipes.

## Files

- **config-feedforward.txt**: Configuration file for the NEAT algorithm.
- **flappy.py**: Main Python script containing the game logic and NEAT implementation.

## Requirements

- Python 3.x
- Pygame
- NEAT-Python

You can install the necessary dependencies using pip:

```sh
pip install pygame neat-python
How to Run
Clone the repository:

sh
Copy code
git clone https://github.com/yourusername/flappy-bird-neat.git
cd flappy-bird-neat
Ensure all the necessary images are in the imgs directory:

bird1.png
bird2.png
bird3.png
pipe.png
base.png
bg.png
Run the game:

sh
Copy code
python flappy.py
Configuration
The config-feedforward.txt file contains the configuration settings for the NEAT algorithm. Below are some key parameters:

NEAT Settings:

fitness_criterion: Criterion for evaluating fitness.
pop_size: Population size.
reset_on_extinction: Whether to reset on extinction.
Genome Settings:

activation_default: Default activation function for nodes.
conn_add_prob: Probability of adding a connection.
conn_delete_prob: Probability of deleting a connection.
Species Settings:

compatibility_threshold: Threshold for species compatibility.
Reproduction Settings:

elitism: Number of top individuals to carry over to the next generation.
Game Logic
The game consists of several components:

Bird: Represents the player character that can jump and fall.
Pipe: Obstacles that the bird must navigate through.
Base: The ground that moves to simulate forward motion.
NEAT Implementation
The NEAT algorithm is implemented using the neat-python library. The neural network controls the bird, and the fitness function rewards the bird for passing through pipes while penalizing it for collisions.

Main Components
Bird Class: Handles the bird's movement and drawing.
Pipe Class: Manages pipe placement, movement, and collision detection.
Base Class: Manages the base movement to simulate a scrolling background.
NEAT Algorithm: Trains the neural network to control the bird.
How to Contribute
Contributions are welcome! Feel free to fork the repository and submit a pull request. You can also open issues for bugs or feature requests.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
The neat-python library for the NEAT algorithm.
Inspired by the original Flappy Bird game.
