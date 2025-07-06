# EvolutionBob

A dynamic and interactive simulation of a virtual ecosystem where different species compete for resources, evolve, and strive for balance. This project was built from the ground up to be a flexible sandbox for exploring complex emergent behaviors in predator-prey and competitive scenarios.

The entire simulation runs in a single HTML file, leveraging modern JavaScript for the logic and Tailwind CSS for a clean, responsive user interface.

![Simulation Screenshot](https://i.imgur.com/rG7gCjS.png)

## The Journey

This simlation was developed iteratively, with each step revealing new, interesting, and often unexpected challenges. We started with a simple grid and three basic species, and through a process of testing, observation, and problem-solving, we identified and overcame several performance bottlenecks and balancing issues. This journey led to the implementation of sophisticated features like spatial grids, hunger mechanics, and search cooldowns, transforming a simple simulation into a robust tool for ecological modeling.

## Features

**Four Unique Species:**
    * **Plants (Producers)**: The foundation of the ecosystem, passively generating energy.
    * **Herbivores (Primary Consumers)**: Feed on plants, converting them into energy.
    * **Carnivores (Secondary Consumers+)**: Specialized hunters that prey on herbivores.
    * **Omnivores (Flexible Consumers)**: Adaptable creatures that eat both plants and herbivores, and can fight carnivores.
* **Tynamic Combat System**: Carnivores and Omnivores will fight if they meet in the same cell. The winner is determined by their current energy, with a configurable combat bonus for the specialized carnivore.
* **Deep Parameter Customization:** A comprehensive "Advanced Parameters" panel gives you granular control over almost every aspect of the simulation:
    * **Energy:** Tune max energy, reproduction thresholds, energy decay, and reproductive costs for each species.
    * **Behavior:** Adjust lifespans, reproduction probabilities, and predator search radii.
    * **AI Chanics:** Fine-tune the "Hunger Threshold" that triggers hunting behavior and a "Search Cooldown" to prevent performance bottlenecks.
* **Interactive Controls:**
    * Adjust grid size from 50x50 up to 250x250.
    * Control the initial population density of each species as a percentage of the map.
    * Change the simulation speed in real-time.
* **Live Data & Analysis:** 
    * A live statistics panel tracks the population of each species and the simulation time.
    * The simulation automatically detects when an ecosystem has collapsed (all organisms have died) and pauses, preserving the final stats for analysis.

## How to Use

1.  **Open `index.html`** in any modern web browser.
2.  **Use the Main Controls:** 
   * **Start/Stop:** Begin or pause the simulation.
    * **Reset All:** Resets the entire simulation with the current settings.
    * **Grid Size:** Adjust the size of the world. The simulation will automatically reset.
3.  **Set Initial Populations:** 
   * Use the sliders to determine the starting percentage of each species. The simulation will reset to apply your changes.
4.  **Tune the Ecosystem:** 
    * Expand the **Advanced Parameters** section to fine-tune the core behaviors of each organism.
    * Experiment with different values to see how they impact the ecosystem's stability and longevity. The simulation will reset automatically as you tune.

## Technology Stack

* **HTML5**
    * **JavaScript (ES6+)**
    * **Tailwind CSS**

## Future Ideas: The Auto-Balancer

The next major step for this project is to implement a **Genetic Algorithm** to automatically find the optimal parameters for long-term stability. This would involve:

1. Creating a "population" of different simulation configurations.
2. Running hundreds of "headless" simulations in the background.
3. Evaluating the "fitness" of each configuration based on its survival time.
4. "Breeding" the most successful configurations and introducing "mutations" to explore new possibilities.
5. Evolving the parameters over many generations to discover the ultimate balanced ecosystem.

This would transform the project from a manual sandbox into a self-optimizing system.