# ZombieEscape

2D top-down zombie survival game built in Unity, featuring a wave-based defense system and an integrated day/night cycle. Currently in active development.

## Overview

ZombieEscape is a top-down survival game where the player defends against waves of zombies across a day/night cycle. The project focuses on stable wave management, reliable enemy spawn logic, and clean gameplay flow.

## Features

- Wave-based defense system with dynamic difficulty scaling

- Integrated day/night manager affecting gameplay conditions

- Smart zombie spawn logic with stable count tracking

- Map boundary control and player movement constraints

- Vehicle mechanics for player mobility

## Tech Stack

- Unity 2D

- C#

- AI-assisted development with Claude

## Notable Engineering Decisions

The zombie counting system was originally implemented with an event-based approach, which led to count desync issues and premature wave-clear triggers. The system was refactored to use a polling-based approach (FindObjectsOfType<ZombieHealth>() at 0.5-second intervals), which resolved the synchronization problems and stabilized wave progression.

Spawner logic and wave-clear triggers were further iterated to handle edge cases around map boundaries.

## Development Approach

This project is built using AI-assisted development. Architectural decisions, gameplay mechanics, and debugging strategy are handled by me. AI tools are used as accelerators during code generation and problem analysis.

## Status

In active development. Unity project files will be added to the repository as the project progresses. Screenshots and gameplay footage will be added once the build stabilizes.

## Author

Mert Baran Yıldırım — Management Information Systems student at Yeditepe University.  
LinkedIn: https://www.linkedin.com/in/mert-baran-yıldırım-7757383b6/
