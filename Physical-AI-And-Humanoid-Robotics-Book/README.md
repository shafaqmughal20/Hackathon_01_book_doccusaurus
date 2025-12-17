# Physical AI & Humanoid Robotics Book

A comprehensive educational resource on Physical AI & Humanoid Robotics, designed for advanced students and developers in AI, robotics, and software engineering working on embodied intelligence and humanoid systems.

## Overview

This book covers the complete pipeline from sensing to reasoning to action in embodied AI systems, with a focus on bridging digital intelligence with humanoid robot bodies through middleware, simulation, perception, and language-driven action.

## Book Structure

The content is organized into four comprehensive modules:

### Module 1: The Robotic Nervous System (ROS 2)
Focus: Middleware for humanoid robot control
- ROS 2 Architecture: Nodes, Topics, and Services
- Bridging Python AI Agents to ROS Controllers with rclpy
- Humanoid Modeling with URDF

### Module 2: The Digital Twin (Gazebo & Unity)
Focus: Physics simulation and environment building
- Physics, Gravity, and Collision Simulation in Gazebo
- High-Fidelity Rendering and Human–Robot Interaction in Unity
- Sensor Simulation: LiDAR, Depth Cameras, and IMUs

### Module 3: The AI-Robot Brain (NVIDIA Isaac™)
Focus: Advanced perception and navigation
- NVIDIA Isaac Sim and Synthetic Data Generation
- Isaac ROS: Hardware-Accelerated VSLAM and Navigation
- Nav2 for Bipedal Humanoid Path Planning

### Module 4: Vision–Language–Action (VLA)
Focus: LLMs integrated with robotics
- Voice-to-Action Systems Using OpenAI Whisper
- Cognitive Planning with LLMs for ROS 2 Action Sequences
- Capstone: The Autonomous Humanoid Robot

## Local Development

To run this documentation site locally:

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```
4. Visit `http://localhost:3000` in your browser

## Build and Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the main branch. The deployment is handled by the GitHub Actions workflow in `.github/workflows/deploy.yml`.

To build the site manually:
```bash
npm run build
```

To serve the built site locally for testing:
```bash
npm run serve
```

## Technologies Used

- [Docusaurus](https://docusaurus.io/): Static site generator optimized for documentation
- [React](https://reactjs.org/): Component-based UI library
- [Node.js](https://nodejs.org/): JavaScript runtime environment
- [GitHub Pages](https://pages.github.com/): Hosting service for the documentation site

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Deployment

The site is deployed at: https://essabel.github.io/Physical-AI-And-Humanoid-Robotics-Book/
